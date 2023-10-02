
 
  
    function getText(filename,fieldname){
    //alert(1)
    var request = new XMLHttpRequest();
    request.open('GET', filename, true);
    request.send(null);
    
    request.onreadystatechange = function () {
        if (request.readyState === 4 && request.status === 200) {
            var type = request.getResponseHeader('Content-Type');
            if (type.indexOf("text") !== 1) {
                document.getElementById(fieldname).innerHTML=request.responseText;
                //alert(request.responseText)
                //return request.responseText;
            }
        }
    }
    
}
window.onload = function () {
    getText('https://fakestoreapi.com/products/categories','catg');
    getText('./assests/products.txt','getdata');
};
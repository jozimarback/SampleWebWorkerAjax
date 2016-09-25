# Sample Web Worker Ajax

Exemplo de um web worker que realiza requisições ajax

Como usar:

var worker = new Worker('workerAjax.js');

worker.addEventListener('message', function ( e ) {
    console.log(e.data);
}, false);

worker.postMessage({url:'urlconsulta',data:null,type:'GET'});

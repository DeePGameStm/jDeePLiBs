# jDeePLiBs
js libs

TEST

Exemples:
Serv{

var deeplib_s = require('./deeplib_s.js');
var server = new deeplib_s.serv();
var io = server.io;

server.addGet('/', 'index.ejs');

io.on('connection', function (socket) {
    //console.log('Un client est connecté !');
    
    socket.on('yop', function(){
        console.log("YOP!"); 
    });
});

server.start(8080);

}

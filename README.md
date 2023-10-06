# calculopropina

Codigo que calcularia la propina de un servicio segun su calidad

function calcularPropina() {
    var nota = +prompt("Por favor, ingresa la nota del mesero (del 0 al 7):");
        if (nota === 0) {
        var reclamo = prompt("Por favor, comparte tu experiencia:");
        console.log("Gracias por tu feedback: " + reclamo);
    } else {
        var propinas = [0, 5, 5, 5, 10, 10, 10, 15];
        var propina = propinas[nota];
        
        var total = +prompt("Ingresa el total de la cuenta:");
        var montoPropina = (total * propina) / 100;

        console.log(`La propina a dejar es de ${montoPropina.toFixed(2)} pesos.`);
    }
}
calcularPropina();

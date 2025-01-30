document.getElementById("bookingForm").addEventListener("submit", function(event) {
    event.preventDefault();

    const name = document.getElementById("name").value;
    const phone = document.getElementById("phone").value;
    const pickup = document.getElementById("pickup").value;
    const dropoff = document.getElementById("dropoff").value;
    const car = document.getElementById("car").value;

    const confirmationMessage = `
        Booking Confirmed!
        Name: ${name}
        Phone: ${phone}
        Pickup: ${pickup}
        Dropoff: ${dropoff}
        Car: ${car}
    `;

    document.getElementById("confirmation").innerText = confirmationMessage;
});

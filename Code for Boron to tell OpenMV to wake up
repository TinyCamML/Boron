#include <Particle.h>

void setup() {
    Serial.begin(9600);
}

void loop() {
    if (Serial.available()) {
        String receivedData = Serial.readStringUntil('\n'); //
        if (receivedData == "Wake up, OpenMV!") {
            // Send a request for data to the OpenMV
            Serial.println("Request data from OpenMV");
        }
    }
    // Process and use the data received from OpenMV here
}


uart = pyb.UART(3, 9600)

while True:
    if uart.any():  # Check if data is available on UART
        received_data = uart.readall()  # Read all available data
        if received_data == b'Request data from OpenMV\r\n':
            # Perform data collection and send it back to the Boron
            data_to_send = setup_data.csv  # Replace with your actual data
            uart.write(data_to_send)  # Send data back to Boron

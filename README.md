### **📱 Send SMS using Arduino via the Internet**

---

### **🌐 Project Overview**

This project demonstrates how to **send SMS messages** using an **Arduino UNO R4** through the **internet** by utilizing the **Circuit Digest SMS API**. The Arduino connects to the internet and, sends a request to the **API endpoint**, and delivers the SMS to the specified phone number.

✅ **Key Features:**

* Send SMS messages using the **Circuit Digest SMS API**

* Internet connectivity is provided through the **ESP32 module present on the Arduino UNO R4 WiFi board.**

* Simple and efficient communication using **HTTP requests**

* Easy-to-build DIY project with minimal components

For the Complete project guide, check our official website \- [https://circuitdigest.com/microcontroller-projects/how-to-send-sms-with-arduino-via-internet](https://circuitdigest.com/microcontroller-projects/how-to-send-sms-with-arduino-via-internet)

---

### **🛠️ Components Required**

* **Arduino UNO R4 WiFi** → Microcontroller for handling SMS operations & Internet Connectivity

* **Power Supply (5V)** → To power the system

---

### **🗂️ Project Structure**

**`/Arduino-SMS-via-Internet`**    
**`├── /Code                  # Arduino sketch (.ino)`**    
**`├── /Circuit-Diagram       # Circuit diagram and wiring illustrations`**    
**`├── /README.md              # Project documentation`**  

---

### **⚙️ Installation and Setup**

#### **1\. Clone the Repository**

**`git clone https://github.com/YogeshwaranP-05/Arduino-SMS-via-Internet.git`**    
**`cd Arduino-SMS-via-Internet`**  

#### **2\. Provide Power Supply for Arduino UNO R4 WiFi**

* **Power the system** with a 5V supply.

#### **3\. API Configuration**

* Get the **Circuit Digest SMS API** link.

* Replace the placeholder in the code with your actual **API key** and **endpoint**.

* Example API format:

**`https://api.circuitdigest.com/sms?api_key=YOUR_API_KEY&number=PHONE_NUMBER&message=YOUR_MESSAGE`**

#### **4\. Upload the Code**

* Open the **`.ino`** file in the **Arduino IDE**.

* Select **Arduino UNO R4** as the board.

* Choose the correct COM port.

* Upload the code to your Arduino.

#### **5\. Run the System**

* Power the system and wait for the ESP32 to connect to the Wi-Fi network.

* The Arduino sends an HTTP request to the **Circuit Digest SMS API**.

* The recipient receives the SMS message.

---

### **📝 Code Explanation**

✅ **Wi-Fi Connection:**

* The **onboard ESP32** connects to the local Wi-Fi network using the provided SSID and password.

✅ **HTTP Request to Circuit Digest SMS API:**

* The Arduino constructs the API URL using the phone number and message.

* It sends an HTTP **`GET`** request to the **Circuit Digest SMS API**.

✅ **Message Delivery:**

* Upon successful connection, the SMS is sent to the specified phone number.

* The console displays a confirmation message.

---

### **🌐 API Usage Example**

**`String apiKey = "YOUR_API_KEY";`**  
**`String phoneNumber = "XXXXXXXXXX";`**  
**`String message = "Hello from Arduino!";`**  
**`String apiUrl = "https://api.circuitdigest.com/sms?api_key=" + apiKey + "&number=" + phoneNumber + "&message=" + message;`**

---

### **🌐 Serial Monitor Output**

**`Connecting to Wi-Fi...`**  
**`Connected to Wi-Fi`**  
**`Sending SMS...`**  
**`SMS Sent Successfully!`**

---

### **🤝 Contributing**

We welcome contributions\! 🎯  
 If you have ideas for improvement or want to add new features:

1. Fork the repository.

2. Make your changes.

3. Submit a pull request.

---

### **🛡️ License**

This project is licensed under the **GPL V3 LICENSE**.  
 Refer to the **`LICENSE`** file for details.

---

### **📧 Contact**

For any queries or suggestions, reach out via:

 🌐 **Official Website:** [Circuit Digest](https://circuitdigest.com)

🚀 **Happy coding and SMS sending\!** 📱


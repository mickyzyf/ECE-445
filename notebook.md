# Yufei Zhu Worklog


# 2021-02-28 - Discussion with Professor Arne Fliflet

After discussing some details regarding design document with Professor Arne Fliflet and TA, our group decided to remove the camera and GPS tracker from the design doc. The existence of  camera might have privacy concerns, and GPS tracker is too expensive for this project.

# 2021-03-7 - Order PCB

We worked on creating PCB board and placed order on PBC way. 

![img](https://lh5.googleusercontent.com/v7fPY-ulhUhbjAOzNBHh4uMG3n1lUzrf0Er4hLmaewP4x1xEORsGph4v9tLe-Ex6qr_0XbNP1pNT_imahKGFDTxHB7CpoCYSgp95GW6EVgb-Srz9BGISKBhDOvi5DCytTkJAPvzItItKGmHVJg)



# 2021-03-14 - Design UI for the phone App

I used Figma to design the UI for the phone App over this week. I do not have too much experience in designing so I found inspiration from Find My app by iphone.

![img](https://lh3.googleusercontent.com/Ism1KArOZiuc2iD1v30F2TvWkbvU5Yq4U__Tz_flFMSINNU3j7S30Z6_BzxYbikcdREZC_OUomzfUYxzq4zJc9Qfnu7TWtsRa0aAczuoLO6Y5ik-5BoauaHAx44TH4RgOn5OotpXi3HkzjEDgA)

# 2021-03-21 - Coded the UI of phone App 

I used React Native to code the mobile phone app. UI of the phone App is done, and most functionalities are done. The actual UI is attached below.

**![img](https://lh5.googleusercontent.com/9P6My1XXR7I9KzUnfcvsCU2QiusMeybcQPx22SuT02I2pEADBPjIcHVBBUYEmUUeSsdJ245NmnhpEu0GPEl98yJfHsiWAK9kA9EWJh7SAInWkCwHm10Yb19-HtKQpDL3GfhhRq9mnT6EthMcSA)**

# 2021-03-28 - Host the Cloud Server

I hosted a NodeJS backed server on Google Cloud Service.  I made server able to handle HTTP GET and POST requests from phone app.

![img](https://lh5.googleusercontent.com/sk3RiEiHIG5w9eatBAI3AQm2OGhaFjthfzMFCg0o-qeBw3UOdOwpEPXFa709iQhh2zukKoJ_NVlDk1wjFa-Raz8aGUyhwfWuiy8XOnyEoCqaGkdugwfseGkRfd4apXqpm61crJwXAG44HAcX5A)

# 2021-04-04 - Program the ESP32 to connect to WIFI and cloud server

![img](https://lh3.googleusercontent.com/Ee8Zvk3atIosYF5p5vQuy_Wi8Fy9xhVqJ5AVX6M1L3skMJ2_OrSdP5WAOwt3uJNkxPX61-l5arFxeayp1IRtp7WCWxVBR1IWEmb_C6Jb-GviW7pDTrcHJElPXpJGNUDpjVOicvignOWS64BPJw)

I program ESP32 using arduino IDE. Using WiFI library, I connect ESP32 to WiFi. Using HTTP library, ESP32 can send and receive data from the cloud server. Blue LED represents the status of the WiFi connection, and red LED represents the status of the security output. In addition, by toggling switches on the phone App, input will be sent to ESP32 over WiFi.

# 2021-04-11 - Test the phone App and ESP32

I used LED to test the system. Using  the timing function of arduino IDE, the average latency for phone app to send data to ESP32 is around 3 seconds. The average latency for ESP32 to send data to phone App is around 5 seconds.

# 2021-04-18 - Integrate Phone app and esp32 to circuitry and PCB.

Worked with teammates to combine all subsystems.
![img](https://lh6.googleusercontent.com/15pDs_B5sKj6z-Fytwyppc26Aj1PIoL_OsK82HPXnx4qKVcOd-AnLyQKns6m3w1rUZusyNtE5LikUiq4JwXV2s-PQYH2NvBLC-GbjYb9LIUpTXLOx1-BmkSQYV97u4TABnL59SXhOhw)

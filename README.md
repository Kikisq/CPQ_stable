#C2C
The name of our app is Click2Cal (C2C). This app allows the user to take a picture of a poster, flyer, or banner of an event. After the image is processed using HPE Haven OnDemand's OCR API, the corresponding date, time, and location of the event is added to the user's calendar. The app allows the user to edit the event details to add any notes or extra information, and save the picture in the event details as a reference.

#Note:
While using an Android phone with a low-res camera, the HPE Haven OnDemand OCR API does not properly recognize text. Unfortunately, that prevents us from parsing accurate date and time information to auto-populate the fields of a new calendar event. In order for us to run a successful OCR, we had to: take a high-quality photo, save it onto the phone, and hardcode the saved photo's filepath. If camera quality was not an issue, we would have run the code on line 159 (below "Real Path") in our CamActivity.java file. Instead, we used the code on line 161 (below "Hardcoded/saved path").

The event poster we ran our code against is: http://imgur.com/lHBE7XD 
The parsed OCR response is: http://imgur.com/oSsuf5T

Developed by: Jay Angel, Kiara Alberto, Priya Kapadia, Sneha Pradhan, and Wonjae Yang

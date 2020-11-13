<img src = "logo.jpg">

Reubus is simply an ML driven Crime Data analyser, Packed with powerful tools for post and pre crime data analysis.
 
## Getting Started 

There are 4 main core functionalities of Reubus 
which is backed by ML:

- Node editor(This section is mainly for viewing the F.I.R. The details of the F.I.R can be represented in nodes.)
- Map predictor(The map section  is used to view the locations of crimes scenes. The ML agent predicts the next possible location and displays in the map)
- Webscraper(This section displays the information of events happened in various locations scrapped from the web.)
- F.I.R filter.The database contains all the records of the F.I.Rs as well as the node information.

*See deployment for notes on how to deploy*


**Implementation Architecture**

• The F.I.R is fed into the application(Reubus).

• The application extracts the information from the F.I.R and stores it in its database.

• The ML agent as been trained with previous data. The agent now inputs the new information from the database and returns the predicted insights and results to the database.

• The application thus collects the information from the database. This include:

1. Who may have done the crime (based on the dataset of convicts we have) ?
2. What may the convict do next (Pattern generation)?
3. A person, the police can consult with who have experience in doing this mode of crime.
• The application then generates a detailed report containing all the above information.                                                                                                                                                                     
### Prerequisites 

Runs on windows only. Needs:

- Python3
- Internet Explorer 11.0

### Installing

Launch the main.au3 file to build from source in Scite or reubus.exe to execute the compiled binary

## Running the tests 

goto [http://localhost:8843](http://localhost:8843)
to check wether the node editor is working.

Open IE and load the maptest.html to rum a check on whether ActiveX is enabled.

### Adding Packages

 Reubus is written in such a way that it can be extended and programmed ,ie more features can be added to it by the user itself.For adding packages make sure the ```package.ini``` is supplied with your GUI application,the application will be embedded inside Reubus while running and can get and transfer data with Reubus

 ``` 
[package]
name=Reubus extension
type=python
 ``` 

If the application to be embedded is in python make sure that POPUP windows style is used for the GUI,for autoit sourcecodes this is not needed.


## Deployment

 Before Launching the app run ``` server_start.bat``` and make sure that ActiveX is enabled ,and Script permissions are given in Internet Explorer

## Built With

* [Autoit](http://www.dropwizard.io/1.0.2/docs/) - Front end GUI
* [Python](https://maven.apache.org/) - Backend ML and server handling
* [Javascript](https://rometools.github.io/rome/) - Communicate with server end and Autoit


**Relevance in future policing**

 The system is built to aid the police department by providing insights on the criminal activities that they handle. It can be used as an effective software to analyze crimes. The software will improve over time by gathering the data. Over time it can gather the information of all criminal activities in the state and find patterns in the crime. When a new crime is reported the software can analyze and compare with existing crime patterns. Thereby, providing valuable insights on the suspect or the next possible action by the suspect. The software also provides features like predicting future crime hotspots and statics of crimes in various places.

 ## Authors 

* **Arjun**-GUI Developer
* **Govind**-ML Developer
* **Surya**-Developer-Integrator
* **Leos**-ML Developer
* **Sandra**-GUI Developer


See list of contributers: [contributors](https://github.com/HacKP-CyberDome/reubus-app/network/dependencies) who participated in this project.

 ## License

 This project is licensed under the **MIT License** - see the [LICENSE.md](LICENSE.md) file for details

 ## Acknowledgments 


* Hat tip to anyone whose code was used as **Inspiration**

# HackGwinnett 6.0 — Project Crawl

**Source:** `hackgwinnett-crawl.json`  
**Projects:** 50

Project descriptions and claims are reproduced from the crawl. Formatting is standardized, repeated team-profile links are deduplicated, and empty crawl markers are removed. Missing section details are marked explicitly. Original wording, spelling, and encoding artifacts are retained.

## Table of contents

1. [Medlexia](#project-medilexa)
2. [Diabetes Preventer for the Blind](#project-diabetes-preventer-for-the-blind)
3. [Prep Time](#project-prep-time-x3g1h9)
4. [CareCompass](#project-carecompass-1donfj)
5. [Medical Jargon Translator](#project-medical-jargon-translator)
6. [Cadence AI](#project-cadence-ai-fa8n04)
7. [Cascade Navigation System](#project-tbd-mfpwt3)
8. [MediBridge](#project-medibridge-hv7tdq)
9. [AccessCare](#project-todo-vbe71s)
10. [AcuPath](#project-acupath)
11. [Siden](#project-maiden)
12. [Clear Case](#project-carebridge-nih7wr)
13. [Visage Health](#project-visage-health)
14. [HealthLens](#project-healthlens-q418rj)
15. ["what should we make our team name"](#project-what-should-we-make-our-team-name)
16. [What if?](#project-what-if-cgfxb1)
17. [Safe Space Stories](#project-safe-space-stories)
18. [CareNori](#project-carenori)
19. [Medical Div](#project-medical-div)
20. [AccessCare](#project-accesscare)
21. [Medicrate](#project-medicrate)
22. [CareFit](#project-carefit)
23. [CareBloom](#project-carebloom-2tvazc)
24. [SMS Shield](#project-sms-shield-gtks0o)
25. [CareBridge](#project-carebridge-504tgi)
26. [CodeRidge_ADHD](#project-coderidge_adhd)
27. [VisitBridge](#project-visit-bridge)
28. [CareBridge Medical Assistant](#project-ringroom)
29. [Beside](#project-beside-tqjhzm)
30. [CareCost](#project-carecost-7j0q23)
31. [AccessAhead](#project-accessahead)
32. [BenefitsBridge](#project-benefitsbridge-d5bzl2)
33. [Pawthfinder](#project-pawthfinder-qagtbu)
34. [Access Care Navigator](#project-access-care-navigator)
35. [Clinic Admitter](#project-clinic-admitter)
36. [Adaptive Touch](#project-adaptive-touch)
37. [Accessible Medical Care Navigator](#project-accessible-medical-care-navigator)
38. [HealthBridge](#project-healthbridge-sif8ny)
39. [Barry](#project-barry-b5adrc)
40. [SimpleJargon](#project-simplejargon)
41. [Memory Preservation Game](#project-memory-preservation-game)
42. [Care Helper](#project-care-helper)
43. [Avaneesh Nelakosigi](#project-avaneesh-nelakosigi)
44. [VisitVoice](#project-visitvoice)
45. [AccessMed](#project-accessmed)
46. [MedVoice](#project-medvoice-koway0)
47. [CareNav](#project-carenav-2zymdw)
48. [Medical Care Voice Navigator](#project-medical-care-voice-navigator)
49. [Wayfind](#project-wayfind-1nd92m)
50. [The Doctor Decoder](#project-the-doctor-decoder)

---

<a id="project-medilexa"></a>
## 1. Medlexia

- **Devpost:** [Medlexia](https://devpost.com/software/medilexa)
- **Crawl ID:** `medilexa`
- **Submitted to:** HackGwinnett 6.0
- **Built with:** flask, python, react

### Team

- [StephenA360](https://devpost.com/StephenA360)
- [Richardson Wajule](https://devpost.com/ykrich)
- [Happya](https://devpost.com/happppya)

### Project links

- [github.com/happppya/Medilexa](https://github.com/happppya/Medilexa)

### Images

- [Image 1](https://d112y698adiu2z.cloudfront.net/photos/production/software_photos/005/765/331/datas/original.jpg)

### Technology references

- [flask](https://devpost.com/software/built-with/flask)
- [python](https://devpost.com/software/built-with/python)
- [react](https://devpost.com/software/built-with/react)

### Project description

### Inspiration

10% of people in the world deal with the struggles of dyslexia on a daily basis. This can make simple tasks from reading a grocery list to reading a medical consent form incredibly difficult, so we sought out to alleviate this problem. We were inspired by extensions like Dyslexia Reader, but we noticed that it wasn't extensible to physical documents. They also lacked integrated TTS features to deliver a seamless experience to dyslexic users. This project brings all those features together along with an AI summary for the best experience.

### What it does

Overall, Medlexia helps dyslexic readers who struggle with interpreting medical documents by appealing to various types of dyslexia (readers who prefer certain fonts and people who prefer listening instead of reading). Start by uploading a PDF with some kind of medical document, and Medilexia not only scrapes the text on the PDF to give text more digestible for people with dyslexia based on professional research, but it allows text to speech options as well as AI generated summaries to allow dyslexic reader to navigate the medical world of documents with ease. Once the original text is generated, the user can customize the options to better fit their needs, catering to the various types of dyslexia a user could have.

### How we built it

We used Vite.js with React and TypeScript for our frontend to create a fast, responsive user interface. The backend is powered by Flask with SQLAlchemy for database management and Flask-CORS for cross-origin requests. We implemented a REST API with full CRUD operations for recipe management, storing step-by-step instructions as JSON arrays in a SQLite database.

We used Vite.js with React for our front end to create a fast, responsive user interface. The backend is powered by Flask and AWS S3 and Lambda to allow for the implementation of AI for our AI summary feature. For the image scraping we used Pytesseract and we used a library called react-text-to-speech for the text to speech feature.

### Challenges we ran into

We had a lot of difficulty linking the backend to an S3 bucket due to permission problems in IAM. We also ran into trouble when trying to fetch the response from our Lambda function back to the Flask backend and then to the frontend.

### Accomplishments that we're proud of

Originally, we set out to focus on developing the core components of the app (uploading a file, scraping text, allowing changed format) and only to leave extra features to if we had more time. Because of our collaborative workflow allowing use to divide the workload efficiently, we were not only able to create an app with the core features, but we were able to add additional features like text to speech and AI implementation.

### What we learned

Our application is a full-stack web-app and it gave us the opportunity to improve both our frontend and backend skills. We got a better sense of creating the architecture of a React application when it comes to what should be made into a component and how to use props and state to make our app more interactive and dynamic. We also learned how to use Amazon Web Services to increase the robustness of our app through the AI feature.

### What's next for Medilexa

After demonstrating our web prototype, Medilexa’s goal is to be ported into mobile apps for accessibility. This can quickly be done with technologies like Ionic Capacitor or React Native. As a mobile app, users would be easily able to scan documents with their phone cameras.

Our already implemented AI summary can be extended into a much more versatile multi-turn conversation feature, using the model’s vision capabilities and understanding to inform users how to interact with forms and allow them to ask more questions.

---

<a id="project-diabetes-preventer-for-the-blind"></a>
## 2. Diabetes Preventer for the Blind

- **Devpost:** [Diabetes Preventer for the Blind](https://devpost.com/software/diabetes-preventer-for-the-blind)
- **Crawl ID:** `diabetes-preventer-for-the-blind`
- **Submitted to:** HackGwinnett 6.0
- **Built with:** opencv, pillow, python, pytorch, react, resnet18

### Team

- [Evan Y](https://devpost.com/evanxyang)
- [Zihong Chen](https://devpost.com/zihongchen0227)

### Images

- [Image 1](https://d112y698adiu2z.cloudfront.net/photos/production/software_photos/005/765/299/datas/original.png)
- [Image 2](https://d112y698adiu2z.cloudfront.net/photos/production/software_photos/005/765/300/datas/original.png)
- [Image 3](https://d112y698adiu2z.cloudfront.net/photos/production/software_photos/005/765/311/datas/original.png)

### Technology references

- [opencv](https://devpost.com/software/built-with/opencv)
- [python](https://devpost.com/software/built-with/python)
- [pytorch](https://devpost.com/software/built-with/pytorch)
- [react](https://devpost.com/software/built-with/react)

### Project description

- Successfully detected snickers

- Successfully detected skittles

- Successfully detected twix

### Inspiration

In the past, we have created an app that helps blind people navigate rooms. It is common for apps to help with navigation, since that is usually the direct result of blindness, but other important aspect like nutrition becomes overlooked. Especially during a time where candy is everywhere (Halloween!) we want to create a way to make sure that blind people can identify types of candy.

### What it does

Our app uses a device's native camera to try to identify candies shown. The device will give a confidence of what it think that type of candy is, and if it passes a certain confidence threshold, it will audibly speak out the type of candy so that blind people can interpret it.

### How we built it

We used python for the machine learning mode and backend. Starting off with the model, we collected data first and consolidated everything into a single folder. Then, we trained the model and had to test several iterations of different types of models to choose the best one. After tuning the model, we implemented some thresholds for real world applications and inserted into a frontend.

### Challenges we ran into

One of the problems was choosing the right model for the AI. At first we used pytorch's linear model, which is poor for the type of data we were training on. Since the data we collected included color and was high dimesnions, we had to use a convelutional neural network. Ultimately, training the network on the data we collected is still not enough to create an accurate model. We finally landed on using a premade model, where we training on our data and reaching proper accuracies.

### Accomplishments that we're proud of

We are proud that the model we training based on the Resnet18 is able to identify the testing data with 100% accuracy in some test. Getting this model to work with open CV is also a big milestone, where it was able to accurately identify 3 different types of candies with a properly tuned confidence threshold.

### What we learned

We learned how to use Resnet18 and pytorch with custom data that we collected ourselves. This is useful since it lets us be able to train other AIs in the future and is not limited to the datasets that are available online.

### What's next for Diabetes Preventer for the Blind

We hope to implement further text to speech so that more information is available.

---

<a id="project-prep-time-x3g1h9"></a>
## 3. Prep Time

- **Devpost:** [Prep Time](https://devpost.com/software/prep-time-x3g1h9)
- **Crawl ID:** `prep-time-x3g1h9`
- **Submitted to:** HackGwinnett 6.0
- **Built with:** custom-tkinter, python

### Team

- [Juan Pablo Chavez](https://devpost.com/juan-pablo-chavez-arenas)

### Project links

- [github.com/jpc23-blip/HG6Project](https://github.com/jpc23-blip/HG6Project)

### Technology references

- [python](https://devpost.com/software/built-with/python)

### Project description

### Inspiration

I have watched many depictions of rare diseases in shows and real life case where a lack of knowledge on a disease can lead to a bad outcome for the patient.

### What it does

The form takes personal data about a user's rare impairment or disease in order to make a standardized document that can be formatted for other healthcare providers

### How we built it

Used python and tkinter to be able to create GUIs

### Challenges we ran into

Because this is my first time using tkinter (and custom tkinter), I struggled with simple parts of creating the program, like using .grid() and .pack().

### Accomplishments that we're proud of

Being able to learn on the fly as I am creating this project.

### What we learned

How to use different functions and attributes in customtkinter and how to make a GUI with python (and in general)

### What's next for Prep Time

Being able to share a program like this to different hospitals and containing a database of different types of diseases can help other healthcare providers prepare for people who may have difficult-to-cure diseases or impairments.

---

<a id="project-carecompass-1donfj"></a>
## 4. CareCompass

- **Devpost:** [CareCompass](https://devpost.com/software/carecompass-1donfj)
- **Crawl ID:** `carecompass-1donfj`
- **Submitted to:** HackGwinnett 6.0
- **Built with:** codex, css, html5, javascript

### Team

- [Tam Nguyen](https://devpost.com/ktram6378)
- [Tristan Escario](https://devpost.com/ravanox1)

### Project links

- [boiledeggisokay.github.io/HackGwinnett6.0](https://boiledeggisokay.github.io/HackGwinnett6.0/)

### Technology references

- [css](https://devpost.com/software/built-with/css)
- [html5](https://devpost.com/software/built-with/html5)
- [javascript](https://devpost.com/software/built-with/javascript)

### Project description

### Inspiration

People with medical disabilities, specifically those that are under recognized are not able to achieve the help that they need, this is because of barriers such as a lack of doctors that are available to aid them and a lack of information regarding their disease. What inspired us to create this tool was to help these people with the medical struggles they face because of their lack of recognition.

### What it does

Our website is comprised of multiple components - The main component being a voice assistant for those with visual impairments who are unable to navigate the website without outside help, a medical decoder in which you can upload medical records and it'll be able to convert it to everyday language, aiding understanding about a user's current health, a specialized search engine for finding specialists and foundations dedicated to helping those with this specific disability, a personalized care plan for those who want to maintain their health at home and also helps schedule appointments and tracks symptoms, and finally, an AI care assistant that looks at a user's current medical situation and is able to make informed responses based on that.

### How we built it

We built it by first drafting a detailed concept of what we're aiming to achieve including who we wanted to help, the judging criteria, and other concepts regarding how to help those with these diseases. Then we ran it through AI and did heavy research on the best solutions and databases for aid in order to further refine the concept and perfect it, then we ran it through GPT Sol 6.1 Codex to create a prototype of the website. After this, we made a log in order to detail beta testing experiences and the mistakes the website has and then used that log to create another prototype and then repeated that process until there was nothing to make a log about.

### Challenges we ran into

We specifically ran into problems with the voice assistant, this includes it picking up noise from itself, background noise, and not being able to identify commands without it being verbatim. We also ran into problems with the voice assistant not being able to detail the website's contents enough to aid those with visual impairments.

### Accomplishments that we're proud of

The agent that is integrated into the medical decoder is successfully able to interpret a various amount of conditions provided to it and outputs a proper simplification of it to those without knowledge of medical jargon, then additionally adds follow ups that detail what steps to take next in regards of the user's health. Another accomplishment that we're proud of is that when entering a health condition into the "Find a specialist" tab, it is able to successfully track down databases that have boatloads of medical information on the condition, and it even gives Google Maps links to medical specialists in the area of the ZIP code that is entered which further enhances user experience.

### What we learned

We learned how to successfully integrate voice detection systems into websites and integrate/use AI to give personalized and detailed feedback when given user information.

### What's next for CareCompass

Expanding the database and care assistant function.

---

<a id="project-medical-jargon-translator"></a>
## 5. Medical Jargon Translator

- **Devpost:** [Medical Jargon Translator](https://devpost.com/software/medical-jargon-translator)
- **Crawl ID:** `medical-jargon-translator`
- **Submitted to:** HackGwinnett 6.0
- **Built with:** numpy, python, tensorflow, transformers

### Team

- [Daniel Clark](https://devpost.com/danc-math)
- [Tanay Gatla](https://devpost.com/tanay-gatla)
- [Dominic Newton](https://devpost.com/dominic-h-newton)

### Technology references

- [numpy](https://devpost.com/software/built-with/numpy)
- [python](https://devpost.com/software/built-with/python)

### Project description

### Inspiration

Sometimes, people have no idea what a doctor is saying because they use big complicated words that only they understand. This is an especially prominent problem for people with disabilities, who need more medical attention overall, and may have difficulty finding answers later. This project will attempt to mediate this problem.

### What it does

Inputs questions relating to medical stuff and outputs accurate and easy-to-understand answers.

### How we built it

Transformers python AI package

### Challenges we ran into

Package not importing right

### Accomplishments that we're proud of

Getting it to actually work without using AI

### What we learned

Disabilities and Healthcare is a difficult concept to program for without using AI

### What's next for Medical Jargon Translator

Give it GUI, maybe get it to automatically detect medical jargon in websites and update the text.

---

<a id="project-cadence-ai-fa8n04"></a>
## 6. Cadence AI

- **Devpost:** [Cadence AI](https://devpost.com/software/cadence-ai-fa8n04)
- **Crawl ID:** `cadence-ai-fa8n04`
- **Submitted to:** HackGwinnett 6.0
- **Built with:** base44, claude, codex, css, javascript, python, react, typescript

### Team

- [Shourya Kaveti](https://devpost.com/shourya23-kaveti)
- [MjtheDj1](https://devpost.com/MjtheDj1)

### Project links

- [spry-my-turn-flow.base44.app](https://spry-my-turn-flow.base44.app/)

### Images

- [Image 1](https://d112y698adiu2z.cloudfront.net/photos/production/software_photos/005/765/180/datas/original.png)
- [Image 2](https://d112y698adiu2z.cloudfront.net/photos/production/software_photos/005/765/187/datas/original.png)
- [Image 3](https://d112y698adiu2z.cloudfront.net/photos/production/software_photos/005/765/190/datas/original.png)
- [Image 4](https://d112y698adiu2z.cloudfront.net/photos/production/software_photos/005/765/193/datas/original.png)
- [Image 5](https://d112y698adiu2z.cloudfront.net/photos/production/software_photos/005/765/201/datas/original.png)

### Technology references

- [css](https://devpost.com/software/built-with/css)
- [javascript](https://devpost.com/software/built-with/javascript)
- [python](https://devpost.com/software/built-with/python)
- [react](https://devpost.com/software/built-with/react)
- [typescript](https://devpost.com/software/built-with/typescript)

### Project description

### Inspiration

I have seen first hand how hard living with aphasia can be. Simple tasks like communicating what they need or having a conversation can become frustrating. The main thing I took away was how it affects your independence.
This inspired us to create Caedance. We focussed on healthcare as it is so important to be able to be understood by others, but often you will get stuck in a loop of calling, filling in forms or fast paced conversations. We wanted to help people engage more with their care.

### What it does

Caedance is a prototype for personalised healthcare communication and navigation for people with Aphasia after a stroke.
The user experience has been designed around images, short keywords and optional speech/text. We want the user to be able to communicate their needs and understand responses whilst linking to appointments, conversations with their care team, transport and follow-ups.

### How we built it

We used Base44 to create the prototype. We used Claude to help us design and improve features. We also used GitHub to help organise our code. We also looked at plugins and skills.
We split the overall idea into smaller interactions. Often when designing the screen we found issues with the design. We were often asking users to type, read or explain something but there wasn’t any support for them to do this.

### Challenges we ran into

The first challenge we faced was deciding what not to include. Whilst an all in one healthcare assistant sounds exciting it was too vague.
The biggest challenge was figuring out how to make the user communicate with the assistant without using fluent speech or writing. We had to think outside the box with the chatbot design to make the assistant personalised, visual and provide support for communication.
We also had to consider when the assistant wouldn’t understand. If the sentence is clear but doesn’t match what the patient wants then it isn’t helpful. We had to make sure we provided a way for the user to say ‘that’s not what I meant’.

### Accomplishments that we're proud of

We are proud of taking a personal idea and creating a prototype with a clearer purpose.
We are particularly proud that we focussed on giving the patients control. We tried to ensure the assistant wasn’t taking over but instead gave the user more control over what they were saying. They could personalise, review and correct what they were saying.
We have improved our collaboration between GitHub, Claude and Base44. We have learnt how to break down our big idea into smaller parts.

### What we learned

We have learnt how to collaborate using GitHub, provide Claude with more useful context, use plugins and skills. We have also learnt how to review what has been created. The biggest thing we have learnt is that accessibility will change the whole interaction. Instead of asking ‘what can the assistant do?’ we asked ‘can the user have control?’

### What's next for Caedance

Next we want to test our prototype with people with aphasia and speech language professionals. We want to know what communication methods are useful, where confusion occurs within the interface and when they would require support from a human.
We also want to improve the links between communication, appointments, transport and follow ups so they feel like one journey.
Whilst Caedance was inspired by my grandpa, his experience can’t represent everyone. We want to take other peoples experiences into consideration.

---

<a id="project-tbd-mfpwt3"></a>
## 7. Cascade Navigation System

- **Devpost:** [Cascade Navigation System](https://devpost.com/software/tbd-mfpwt3)
- **Crawl ID:** `tbd-mfpwt3`
- **Submitted to:** HackGwinnett 6.0
- **Built with:** gemini, jsx

### Team

- [Kingston Dempsey](https://devpost.com/kingstonldempsey)
- [Ethan M](https://devpost.com/ethankaim0205)

### Technology references

- [gemini](https://devpost.com/software/built-with/gemini)

### Project description

### Inspiration

Our project is inspired by our biology. Cells use information cascades to run billions of processes per minute with an astounding lack of error. By establishing error identification between each step of appointment applications, we mimic the efficiency of our biology.

### What it does

It provides a streamlined interface that guides both disabled and general patients to the exact resources they need to secure an appointment with a professional that works for them and understands their needs. It removes the cluttered information barrage that many current application systems have.

### How we built it

We built a frontend system with AI resources that includes a professional page and a patient page, coding in JSX to increase efficiency and debugging through scrutiny. We also built a backend system that saves patient profiles to a database, assigns them unique usernames and passwords, and allows specific professionals to access their patients' profiles.

### Challenges we ran into

There were many bugs with the visual AI frontend, but we used knowledge of pixel math and sine waves to fix the visual issues.

### Accomplishments that we're proud of

It was a real task to complete such a large project as a team of just two, both at our first Hackathon ever. The experience was fun and gave us a look into the real life of a software developer.

### What we learned

AI is an extremely powerful tool, but becomes even more effective when paired with human creativity and deliberation.

### What's next for Cascade Navigation System

We can continue to develop the security of our system and perhaps eventually market it to Wellstar, an important hospital in our area.

---

<a id="project-medibridge-hv7tdq"></a>
## 8. MediBridge

- **Devpost:** [MediBridge](https://devpost.com/software/medibridge-hv7tdq)
- **Crawl ID:** `medibridge-hv7tdq`
- **Submitted to:** HackGwinnett 6.0
- **Built with:** ocr, opencv, pytesseract

### Team

- [loloheria Hung](https://devpost.com/loloheria)
- [Cloudy Sanjesh](https://devpost.com/ishaan-sanjesh)
- [Aarmaan Singh](https://devpost.com/aarmaansingh-prof)

### Project links

- [github.com/Singham64/medibridge](https://github.com/Singham64/medibridge)

### Technology references

- [opencv](https://devpost.com/software/built-with/opencv)

### Project description

### Inspiration

According to the Centers for Disease Control and Prevention (CDC), approximately 1 in 21 U.S. adults reported a vision disability in an earlier national study (CDC, 2025). For these individuals, navigating the healthcare system can present challenges, especially when important information is provided through printed documents.

Although assistive technologies such as screen readers and text-to-speech applications already exist, we wanted to create something specifically focused on healthcare accessibility. Our goal was to make medical documents easier to understand and improve communication between patients and healthcare providers. This inspired us to develop MediBridge, a web application designed to help bridge the accessibility gap in healthcare.

### What it does

MediBridge is a healthcare accessibility application designed primarily for patients with visual or hearing impairments. The application allows users to upload images of medical documents, such as doctor's notes, treatment plans, and appointment instructions. It extracts the text from these documents and displays it in a readable format. For visually impaired users, MediBridge includes a text-to-speech feature that reads the extracted information aloud. Users can start, pause, resume, or stop the audio, allowing them to listen at their own pace. Additionally, MediBridge includes a live-captioning feature designed for deaf or hard-of-hearing patients. By converting spoken words into text, the application can help users follow conversations with healthcare providers or hospital staff. Together, these features aim to make navigating medical information and communicating in healthcare environments more accessible.

### How we built it

We developed MediBridge using Python, Flask, HTML, CSS, and JavaScript. The backend uses Flask to handle document uploads and connect the user interface to our optical character recognition (OCR) system. We used OpenCV for image processing and Tesseract OCR to recognize and extract text from uploaded medical documents. Once the text is extracted, it is sent back to the frontend, where JavaScript's built-in Speech Synthesis API allows users to listen to the document. For live captions, we implemented the browser's Web Speech Recognition API, which converts spoken audio into text in real time. We also designed a simple, high-contrast interface with clearly labeled buttons and separate sections for document scanning, audio controls, and live captions. Our focus was on keeping the application lightweight, accessible, and easy to navigate without requiring complicated setup or specialized hardware.

### Challenges we ran into

One of our biggest challenges was implementing accurate document scanning. Medical documents can contain different layouts, font sizes, and formatting, making text extraction difficult. We experimented with image preprocessing techniques using OpenCV to improve the quality of the text recognized by Tesseract. Another challenge was connecting our Python-based OCR system to the web interface. We had to learn how to use Flask to accept uploaded images, process them, and return the extracted text to the browser. We also encountered browser compatibility issues while developing the live-captioning feature. Speech recognition was not supported in our original browser, Zen, so we tested the functionality in Google Chrome, where it worked successfully. These challenges taught us the importance of testing individual components before integrating them into a complete application.

### Accomplishments that we're proud of

Our biggest accomplishment was building a functional healthcare accessibility application within the limited time available during the hackathon.We successfully integrated three major features into one web application:

- OCR document scanning: Extracting text from uploaded medical documents.

- Text-to-speech: Reading extracted information aloud with playback controls.

- Live captions: Converting spoken instructions into readable text.

We are especially proud that these features address different accessibility needs while remaining straightforward to use. Rather than building an overly complicated application, we focused on creating a working prototype that demonstrates how relatively simple technologies can help make healthcare more inclusive.

### What we learned

Through MediBridge, we gained hands-on experience developing a full-stack web application and connecting multiple technologies.
We learned how Flask handles communication between a Python backend and a JavaScript frontend, how OCR works with image-processing techniques, and how browser-based speech APIs can be used to build accessibility features.
We also learned that accessibility involves more than simply adding assistive features. Interface design, browser compatibility, readability, and ease of use are all important considerations.
Most importantly, we learned how to prioritize essential features and build a functional product under time constraints.

### What's next for MediBridge

We would like to expand our application to cognitively impaired patients, as this is the greatest disability in the United States (source, year). If the patient is elderly or has difficulty remembering, the app will have an option to create a to-do list from action items listed from the inputted document. This will be able to be printed and downloaded, so that it can be carried around without requiring the app to stay open or for users to repeatedly operate the app. This will also address the privacy issue, because then data does not need to be retained for long periods of time. If medical information remains stored in an app for long periods of time, there is a risk for data leakage/vulnerability. Therefore, chats will not be stored for over 24 hours. Additionally, the models used are local, so the data does not go to a cloud. Finally, we would like to expand to support multiple languages, as the US is a diverse country, with about 8.4% of the population having limited English proficiency (People That Speak English Less than “Very Well” in the United States, 2020).

---

<a id="project-todo-vbe71s"></a>
## 9. AccessCare

- **Devpost:** [AccessCare](https://devpost.com/software/todo-vbe71s)
- **Crawl ID:** `todo-vbe71s`
- **Submitted to:** HackGwinnett 6.0
- **Built with:** cloudflare, react, workers

### Team

- [Nikolas Dyer](https://devpost.com/Nik-Sharp)

### Technology references

- [cloudflare](https://devpost.com/software/built-with/cloudflare)
- [react](https://devpost.com/software/built-with/react)

### Project description

### Inspiration

TeleHealth is a new innovation in healthcare technology, which allows patients to seek healthcare without having to take time out of their day to go to a hospital, but instead they can do it from the comfort of their phone or laptop.

Sadly, current telehealth technology has problems: many solutions have poor accessibility, including insufficient screen reading technology (57% of visually impaired people have had issues accessing telehealth solutions), poor captioning (40% of top-20 US hospitals used telehealth platforms that routinely offered automatic captioning), and more.

### What it does

AccessCare is designed to incorporate accessibility. A couple of important notes:

- WCAG 2.1 Level AA accessibility compliance, which is (soon to be) legally required in hospitals.

- Better Captioning. We provide this with two features: two transcription models are run (note that during the demo, to better showcase this, we run whisper against a mock) against eachother, if there's any differences between them, it gets flagged so either the provider or another person in the call (excluding the patient, there are designated people that can be added as well for this) can select the correct transcription. Another safeguard against incorrect captioning is having the provider /  other person review the transcript while it's happening, if changes are needed they can issue a correction.

- For patients with speech disabilites / who require external devices to type, we implement multiple features. We firstly provide them with a built in speech board that has multiple options for them to select, which can be prewritten before the meeting or can also be done  by AI during the meeting, which will listen to the conversation and provide suggestions. Additionally, patients can type less (e.g "daily dosage" instead of "How much dosage do I need daily")

### How we built it

Tech stack is built on React and Cloudflare Workers, with Bedrock used as the AI model endpoint (workers AI is used for the transcription models). Claude Code and Antigravity were used for the implementation, and Claude Code was used for architecture discussion and general ideation (with my input of course).

### Challenges we ran into

My Claude Code sub ran out of usage, didn't realize that the cloud would be so slow so I switched to antigravity for the last minute implementation.

### Accomplishments that we're proud of

I was really locked in during this.

### What we learned

Start my 5 hour limit earlier so I don't have to worry about running out of usage mid hackathon :(

### What's next for AccessCare

HIPPA compliance, better implementation

(for full transparency, if it's not clear from the video, most implementation was not completed)

---

<a id="project-acupath"></a>
## 10. AcuPath

- **Devpost:** [AcuPath](https://devpost.com/software/acupath)
- **Crawl ID:** `acupath`
- **Submitted to:** HackGwinnett 6.0
- **Built with:** aruco, claude-code, cloudflare-tunnel, fastapi, html5, javascript, opencv, python, pytorch, three.js, ultralytics, uvicorn, web-audio-api, web-speech-api, yolo26

### Team

- [Jasper Chen](https://devpost.com/jasper-chen)
- [Brian Li](https://devpost.com/prodyradstudios)
- [Ayan Sandybayev](https://devpost.com/ayan-s-learn)

### Project links

- [drive.google.com/file/d/16EVZeWiPle5Bxcwt1NcgwMIfLEhC560z/view](https://drive.google.com/file/d/16EVZeWiPle5Bxcwt1NcgwMIfLEhC560z/view?usp=sharing)
- [www.cdc.gov/vision-health-data/prevalence-estimates/vision-loss-prevalence.html](https://www.cdc.gov/vision-health-data/prevalence-estimates/vision-loss-prevalence.html)
- [rehab.jmir.org/2025/1/e64666](https://rehab.jmir.org/2025/1/e64666)
- [jasperwchen.github.io/JABCross](https://jasperwchen.github.io/JABCross)
- [github.com/jasperwchen/JABCross](https://github.com/jasperwchen/JABCross)

### Technology references

- [html5](https://devpost.com/software/built-with/html5)
- [javascript](https://devpost.com/software/built-with/javascript)
- [opencv](https://devpost.com/software/built-with/opencv)
- [python](https://devpost.com/software/built-with/python)
- [pytorch](https://devpost.com/software/built-with/pytorch)
- [three-js](https://devpost.com/software/built-with/three-js)

### Project description

VIDEO LINK: https://drive.google.com/file/d/16EVZeWiPle5Bxcwt1NcgwMIfLEhC560z/view?usp=sharing

### Inspiration

Google Maps gets you to the front door of a hospital, then it stops. Inside, there is no GPS, the corridors look alike, and the directions are printed on signs. For a blind patient, that usually means depending on whoever happens to be nearby.

The CDC estimates that over 7 million Americans live with vision loss or blindness, about 1 million of them blind (CDC). Researchers at Michigan Medicine note that blind and low-vision patients face disability-related barriers in health care settings, and their response was to train staff as human guides (JMIR, 2025). We wanted to know if a phone could give a patient that kind of guidance on their own.

### What it does

JabCross is indoor navigation for blind and low-vision patients. The patient wears a phone on their chest with the camera facing forward, taps once to start, taps the mic, and says something like "take me to radiology."

From there the app talks them through the route:

- Directions: "Turn right about 90 degrees," then "Walk forward about 7 steps."

- Safety: if something is less than about 1 meter ahead, it plays a tone, says stop, and says which side has more space.

- Bad camera view: if the lens is covered, it tells the patient to fix the phone.

- Location: printed markers on the walls tell the app exactly where the patient is.

- Arrival: it announces each destination out loud.

Patients can also ask "where am I," "repeat," "stop," or "cancel." Destinations understand everyday words, so "radiology," "imaging," and "x-ray" all lead to the same place.

### How we built it

Phone. A plain HTML and JavaScript page sends a camera frame and compass heading to a laptop about every 300 ms, and speaks the replies. It uses the browser's speech recognition and speech synthesis, Web Audio for alert tones, and a wake lock so the screen stays on. A Cloudflare tunnel provides the HTTPS connection that phone cameras require.

Perception. A FastAPI server runs the Ultralytics YOLO26 depth model on each frame. It finds the nearest distance in meters in the left, center, and right thirds of the view, ignoring the bottom quarter so the floor does not count as an obstacle. OpenCV detects ArUco markers, which are printed black and white squares, and solvePnP turns each one into a distance and a bearing.

Navigation. Our navigator holds a graph of the building, finds the shortest route, and decides what to say. Safety always comes first: blocked camera, then obstacle, then turn correction, then the next marker, then walking. A marker sighting overrides the app's estimate of position. It also corrects the compass.

Map and viewer. We started from the real Grady Memorial Hospital ground floor plans, then built a staged four-stop route for filming: Entrance, Lobby, Pharmacy, X-ray. The same map file drives the navigator and a Three.js viewer. The hospital walkthrough in our video is a scripted simulation shown beside the real phone footage. It does not track the phone live.

### Challenges we ran into

- Knowing where you are without GPS. Depth tells you what is in front of you, not where you are. That is why we added printed markers, which give an exact position at each stop.

- Depth was fooled in two ways. Stretching each frame into a square made indoor scenes read about 24% too far away on the NYU Depth V2 dataset, so we kept each frame's real shape. The model also reports a smooth wall about 1 meter away when the lens is covered, so we check image contrast separately.

- Too much talking. Our first version repeated instructions every 3 seconds, which is exhausting when speech is your only interface. We rebuilt it to speak only when something changes. A patient must drift more than 30 degrees to get a correction, then return within 15 degrees to clear it. An obstacle must show up in two frames in a row to trigger a stop, and the path must open past 1.3 meters to end it.

- Close markers can mislead.** Standing slightly off to one side of a nearby marker skews its bearing, so we only correct the compass from markers more than 2 meters away.

- iPhone permissions. Camera, motion, and audio all need a real tap, so one start button has to unlock all of them at once. We planned always-on listening, then settled on tap to talk, which also stops the app from transcribing its own voice.

### Accomplishments that we're proud of

The navigator has 50 automated tests that replay simulated camera readings, including obstacles, missed markers, and arrivals, so we could develop it before the perception code existed. We are also proud of how quiet it is. Saying less took more engineering than saying more.

### What we learned

For someone who cannot see the screen, the interface is timing. A correct instruction at the wrong moment is still a bad instruction. We also learned to pair two imperfect signals: a printed marker is exact but occasional, a compass is constant but drifts, and each one covers for the other.

### What's next for JabCross

- Test with blind and low-vision users, and with orientation and mobility specialists.

- Calibrate step counts and depth distances in real hallways.

- Run a pilot in one real hospital corridor. Our Grady geometry is illustrative and has not been validated for real navigation.

- Replace printed markers with camera-based recognition of the location, so hospitals need no new signage.

- Add routes for other disabilities, such as step-free routes for wheelchair users.

---

<a id="project-maiden"></a>
## 11. Siden

- **Devpost:** [Siden](https://devpost.com/software/maiden)
- **Crawl ID:** `maiden`
- **Submitted to:** HackGwinnett 6.0
- **Built with:** amazon-web-services, claude, claudecode, opus, visual-studio

### Team

- [Aiden Byun](https://devpost.com/aidenbyun528)
- [Atharv Kasliwal](https://devpost.com/snapnaps123mc)
- [Serge Laguerre](https://devpost.com/sergeno0909)

### Project links

- [proposals-kept-frank-transportation.trycloudflare.com](https://proposals-kept-frank-transportation.trycloudflare.com/)
- [drive.google.com/drive/folders/16PsclM6Rk7jqyja0le7yLnAHtYYnidsu](https://drive.google.com/drive/folders/16PsclM6Rk7jqyja0le7yLnAHtYYnidsu?usp=share_link)

### Images

- [Image 1](https://d112y698adiu2z.cloudfront.net/photos/production/software_photos/005/765/050/datas/original.png)
- [Image 2](https://d112y698adiu2z.cloudfront.net/photos/production/software_photos/005/765/051/datas/original.png)
- [Image 3](https://d112y698adiu2z.cloudfront.net/photos/production/software_photos/005/765/052/datas/original.png)
- [Image 4](https://d112y698adiu2z.cloudfront.net/photos/production/software_photos/005/765/054/datas/original.png)
- [Image 5](https://d112y698adiu2z.cloudfront.net/photos/production/software_photos/005/765/055/datas/original.png)
- [Image 6](https://d112y698adiu2z.cloudfront.net/photos/production/software_photos/005/765/056/datas/original.png)
- [Image 7](https://d112y698adiu2z.cloudfront.net/photos/production/software_photos/005/765/057/datas/original.png)
- [Image 8](https://d112y698adiu2z.cloudfront.net/photos/production/software_photos/005/765/304/datas/original.png)
- [Image 9](https://d112y698adiu2z.cloudfront.net/photos/production/software_photos/005/765/306/datas/original.png)
- [Image 10](https://d112y698adiu2z.cloudfront.net/photos/production/software_photos/005/765/309/datas/original.png)
- [Image 11](https://d112y698adiu2z.cloudfront.net/photos/production/software_photos/005/765/310/datas/original.png)
- [Image 12](https://d112y698adiu2z.cloudfront.net/photos/production/software_photos/005/765/313/datas/original.png)

### Technology references

- [amazon-web-services](https://devpost.com/software/built-with/amazon-web-services)
- [visual-studio](https://devpost.com/software/built-with/visual-studio)

### Project description

### Inspiration

We heard from disabled patients who face a constant stream of forms, prescriptions, appointments, and paperwork. Navigating the healthcare system is already confusing, and for people with disabilities it can become overwhelming. We wanted to build something that makes getting care simpler and more organized.

### What it does

Siden is an AI-powered assistant that turns your medical documents and conversations into an organized health record. It keeps track of prescriptions, hospital visits, upcoming forms, doctors, and other medical data. You can add information by scanning documents or by telling the app through voice or text.

Siden is designed with accessibility first:

- Read-aloud support: Key parts of the interface are spoken during conversations with the AI.

- Easy voice control: Start talking by clicking the circle or pressing the space bar.

- Paperwork help: Siden can fill out necessary forms and write doctor's notes, cutting down on repetitive work.

- Medication reminders: Prescriptions come with timed notifications and all their details saved in one place.

- Separate accounts: Users can have multiple accounts so that an entire family can keep track of their information in one easy to access website.

- Priorities: Users can see what actions are most urgent, and can easily access instructions on what to do about them, deadlines, and can use our platform to fill out necessary forms, letters, and even add reminders to ones Google Calendar Account.

### How we built it

We built Siden with Claude Code, using models including Fable and Opus. We wrote detailed, carefully structured prompts to make the experience work well for blind users.

### Challenges we ran into

- Claude Code took a long time to generate each piece of the program, so we had to write efficient prompts and make every one count.

- Claude Code was often wrong about its own output, so we had to step in and adjust the code by hand.

### Accomplishments that we're proud of

- Voice-based interaction that makes the app easy to use hands-free

- Ways for Siden to help by writing notes, letters, etc.

- Multiple profiles, so families can use Siden together

- A prioritization system for notifications, so the most important reminders come first

### What we learned

We started out expecting Claude to do most of the work, but quickly found that it struggled to "see" what the program looked like. We had to write clear descriptions of the interface so it knew what to fix. We also learned how to use Chain-of-Thought prompting to get better results from each prompt.

### What's next for Siden

Right now, Siden is optimized for blind, deaf, and colorblind users, with the voice control, text options, and colorblind settings. Next, we plan to expand support to other disabilities so that even more patients can navigate healthcare with confidence.

---

<a id="project-carebridge-nih7wr"></a>
## 12. Clear Case

- **Devpost:** [Clear Case](https://devpost.com/software/carebridge-nih7wr)
- **Crawl ID:** `carebridge-nih7wr`
- **Submitted to:** HackGwinnett 6.0
- **Built with:** claude

### Team

- [Infernalitiy Ho](https://devpost.com/Infernalitiy)
- [sihe1230-gif](https://devpost.com/sihe1230-gif)
- [Daniel Jiang](https://devpost.com/dj87why)

### Project links

- [github.com/Infernalitiy/clearcase](https://github.com/Infernalitiy/clearcase)

### Images

- [Image 1](https://d112y698adiu2z.cloudfront.net/photos/production/software_photos/005/765/244/datas/original.png)
- [Image 2](https://d112y698adiu2z.cloudfront.net/photos/production/software_photos/005/765/245/datas/original.png)
- [Image 3](https://d112y698adiu2z.cloudfront.net/photos/production/software_photos/005/765/246/datas/original.png)

### Project description

### Inspiration

Medical paperwork is written for people who can read small print, decode jargon, make phone calls, and have the energy to do all of it. I've watched family members struggle to understand bills and letters from the healthcare system, and for disabled patients those barriers stack up: a blind patient can't read a denial letter, a Deaf patient can't "call the number below," and a patient with a learning disability gets a wall of jargon. Missing a deadline or misunderstanding instructions can cost someone their care or their coverage.

### What it does

CareBridge takes one medical document (a bill, an insurance denial, discharge instructions) and turns it into the format that works for that specific person:

- Blind / low vision: read aloud in short pieces, with large high-contrast text and screen-reader support

- Deaf / hard of hearing: text only, with no audio dependence and a drafted message instead of "call this number"

- Cognitive / learning disabilities: very short, simple steps, one card at a time, with a dyslexia-friendly font option

- Fatigue / motor limits: a minimal-effort checklist with big buttons

Interrupt and ask: at any moment, even in the middle of being read aloud, the user can stop and ask a question ("What does this mean?", "Say it simpler"). CareBridge answers only from the document, quotes the exact line, and resumes where they left off. If the document doesn't say, it says so instead of guessing.

Verify, don't trust: every card has a "Show original" link, and amounts, dates, and medication names are flagged to double-check with a real person.

### How we built it

- A Flask backend calls Claude through Amazon Bedrock (vision) to read the document image and return structured JSON: facts, deadlines, next steps, and the exact original text for each fact

- A plain HTML/CSS/JavaScript frontend renders the same JSON differently for each disability profile

- The browser's speech synthesis handles read-aloud, one short chunk at a time, with our own position tracking

- The question-answering step is grounded in the document and returns a source quote

- Sample documents are fictional and cached, so the demo works without an API key

### Challenges we ran into

- Browser speech synthesis is unreliable for pausing and resuming, so we track our own position and speak one short chunk at a time

- Keeping simple language from changing the meaning, which is why every card links back to the original text

- Making answers stay inside what the document actually says

- Building for several different access needs without making the interface cluttered

### Accomplishments that we're proud of

- The interrupt-and-ask flow, which fits how people actually read confusing paperwork

- The same document producing very different, useful outputs for different users

- Keyboard-only navigation and screen-reader announcements throughout

### What we learned

Accessibility is not one setting. Different disabilities need different shapes of information, not just bigger text. We also learned how important it is to show a model's sources instead of asking users to trust it.

### What's next for CareBridge

- Test with disabled users and accessibility experts. We have not done user testing yet, and that is the most important next step

- Support PDFs and multi-page documents

- Offer clinics and insurers a way to send the accessible version automatically

- Add a reply helper that drafts accommodation requests and appeal letters

- Add more languages

---

<a id="project-visage-health"></a>
## 13. Visage Health

- **Devpost:** [Visage Health](https://devpost.com/software/visage-health)
- **Crawl ID:** `visage-health`
- **Submitted to:** HackGwinnett 6.0
- **Built with:** javascript, react, typescript

### Team

- [Shaurya Dave](https://devpost.com/shauryadave09)
- [Ken Dang](https://devpost.com/k-dan-g59192)
- [Christian Djiofack](https://devpost.com/gaminglemonz)

### Project links

- [github.com/gaminglemonz/hack-gwinnett-6](https://github.com/gaminglemonz/hack-gwinnett-6)

### Technology references

- [javascript](https://devpost.com/software/built-with/javascript)
- [react](https://devpost.com/software/built-with/react)
- [typescript](https://devpost.com/software/built-with/typescript)

### Project description

### Inspiration

One of our teammates’ mothers works as a doctor in a hospital, assisting the paralyzed.

### What it does

We made software for paralyzed people in hospitals to have an interface related to their needs and wants during their time there.

### How we built it

We searched for multiple hours for a facial recognition API. After all of that, we found one that fulfilled our needs on GitHub, and we implemented it. We also used JavaScript, TypeScript, and React to code the entire interface, controls, and integration of the facial recognition software.

### Challenges we ran into

A challenge was that cursor movement relative to the moving face was not actually inputting how we wanted it to.

### Accomplishments that we're proud of

We were finally able to make software that accurately reads facial input and could improve the lives of paralyzed people while hospitalized. This took a very long time, but we pulled it off.

### What we learned

We learned how to manage time under the harsh deadline and adapt quickly under the pressure of a clock.

### What's next for Visage Health

We plan to expand and improve on this by adding an on-screen keyboard capable of multiple key presses simultaneously. This could lead to numerous additions relating to quality of life.

---

<a id="project-healthlens-q418rj"></a>
## 14. HealthLens

- **Devpost:** [HealthLens](https://devpost.com/software/healthlens-q418rj)
- **Crawl ID:** `healthlens-q418rj`
- **Submitted to:** HackGwinnett 6.0
- **Built with:** ai

### Team

- [Sungjae Lee](https://devpost.com/lakesuwa)
- [Aarav Sandeep Gaudana](https://devpost.com/agaudana)
- [Yixiang520 chen](https://devpost.com/Yixiang520)

### Project links

- [healthlens-xbzp.onrender.com](http://healthlens-xbzp.onrender.com/)
- [github.com/agaudana/hackgwinnett-6.0](https://github.com/agaudana/hackgwinnett-6.0)

### Images

- [Image 1](https://d112y698adiu2z.cloudfront.net/photos/production/software_photos/005/765/059/datas/original.png)
- [Image 2](https://d112y698adiu2z.cloudfront.net/photos/production/software_photos/005/765/061/datas/original.png)
- [Image 3](https://d112y698adiu2z.cloudfront.net/photos/production/software_photos/005/765/060/datas/original.png)
- [Image 4](https://d112y698adiu2z.cloudfront.net/photos/production/software_photos/005/765/062/datas/original.png)
- [Image 5](https://d112y698adiu2z.cloudfront.net/photos/production/software_photos/005/765/063/datas/original.png)
- [Image 6](https://d112y698adiu2z.cloudfront.net/photos/production/software_photos/005/765/064/datas/original.png)
- [Image 7](https://d112y698adiu2z.cloudfront.net/photos/production/software_photos/005/765/065/datas/original.png)

### Project description

- Initial onboarding screen for HealthLens, where users learn how to use the app and choose settings for viewing.

- Take a picture of a pill or a prescription bottle here.

- Prescription brief description based only on what we can see.

- Urgent instructions given in the doctors notes

- upload doctors notes or discharge instruction

- To-do based on doctors papers

- Take a picture- dark mode

### Inspiration

Upon hearing the topic, we talked about how paper instructions from hospitals were too difficult to read.
We also talked about how pills got mixed up when storing them in cabinets, and how we forgot whose or how to take the medicine.

### What it does

Imagine a dyslexic person. A doctor hands them piles on top of piles of medical information, as well as a number of prescriptions. How are they supposed to independently dissect what has been given to them?

HealthLens turns confusing medical info into shorter and clearer steps you can read or listen to.

- Explain a paper: take a photo of discharge instructions or doctor's note, or rtype words in. HealthLens reads the text and rewrites it in plain language, going one step at a time. The steps are sorted by urgency.

- tap any medical lingo to see what it means

- read aloud: every step, every sentence, or the whole page can be spoken

- What is this pill? Takea  photo of a pill or prescription bottle and HealthLens tells you what it is , what its for, how to take it (ONLY IF PROVIDED ON THE PRESCRIPTION) and what to be careful out, in concise lines

- Built for different readers with options for larger text, wider spacing, OpenDyslexic font, and high contrast themes

- Add to calendar: medicine times and follow-up appointments exported to an .ics file

### How we built it

Frontend: React+Typescript+Vite, large button, step by step interface. Read aloud uses browsers built in speech ability
Backend: Node.js + Express. Photos read with Tesseract.js

-AI: all through amazon bedrock, called only from the server

-gpt-oss-120b to turn doc text into plain language, steps, word definitons

-Claude Sonnet 5.5 (vision) looks at pill and bottle photos

-Demo mode if AI is unavailale, app shows clearly labeled sample answers, instead of crashing

-Testing and deployment: wrote 58 tests and deployed both halves to Render

- worked in parallel on separate branches with written API Contract between frontend and backend for concurrent development

### Challenges we ran into

-text AI couldnt see images -- existing bedrock access also included vision model Claude, so added it without a new provider and updated API Contract

-Phone photos were too big -- bedrock rejects photos above 3.75mb, so we now shrink photos in browser before uploading

- answers were way too long! we cater to different readers! we set strict word limits and split the screen into three labeled lines aiming for ~30 words

### Accomplishments that we're proud of

- A full working path to photo to plain words to read aloud, deployed and usable in JUST 5 hours of work time

- pill id correctly reads real bottle labels and print imprints, and honeslty admits when not sure

- interface designed for people who struggle with text: bg buttons, short sentences, everything spoken

- safety rules enforced in code, plus labeled demo

-58 automated test

### What we learned

-accessibility is mostly about cutting

-ai output cant be trusted as is- check it, rebuild, enforce rules yourself

- "I'm not sure, ask a pharmacist" prevents us from going to jail

- agreeing on an API Conract early saved us

### What's next for HealthLens

-more languages for ESL patients

-Pill reminders

-Checking pill identification against official drug db

- medicine cabinet - which pill belongs to who based on discharge notes

- testing with real users with cognitive disabilities

-more paper types for support

---

<a id="project-what-should-we-make-our-team-name"></a>
## 15. "what should we make our team name"

- **Devpost:** ["what should we make our team name"](https://devpost.com/software/what-should-we-make-our-team-name)
- **Crawl ID:** `what-should-we-make-our-team-name`
- **Submitted to:** HackGwinnett 6.0
- **Built with:** gemini, visual

### Team

- [AndrewV16K Joseph](https://devpost.com/AndrewV16K)
- [Lewis Yang](https://devpost.com/masterop0514)

### Project links

- [sites.google.com/view/medicalaccessibilitysystem/full-page-embed](https://sites.google.com/view/medicalaccessibilitysystem/full-page-embed)
- [drive.google.com/file/d/1ntlnACZmVHsr8XMbCcplusa6lm0hHWus/view](https://drive.google.com/file/d/1ntlnACZmVHsr8XMbCcplusa6lm0hHWus/view)

### Technology references

- [gemini](https://devpost.com/software/built-with/gemini)

### Project description

### Inspiration

Inspired by the real-world barriers patients face when trying to navigate complex hospital systems, locate verified accessible facilities, and arrange reliable medical transportation in Gwinnett County.

### What it does

The Medical Accessibility System is an all-in-one digital hub for Gwinnett County residents that provides:

Verified Healthcare Directory: Over 16 local hospitals, urgent cares, dental clinics, and orthopedics with verified accessibility data (parking, ramp inclines, automated doors).   

Ride Gwinnett & NEMT Dispatch: A streamlined booking tool for ADA paratransit and private lift-van medical transport.   

Indoor Micro-Navigation: An interactive spatial map that plots accessible indoor routes while dynamically bypassing stairs or broken elevators.   

Custom Accessibility Profiles (DUAP): Personalized mobility and sensory settings that tailor routes and system alerts to individual needs.   

### How we built it

Frontend: Built with HTML5, Tailwind CSS, and custom JavaScript for real-time filtering, interactive canvas mapping, and accessibility toggles.

Accessibility Enhancements: Integrated high-contrast mode overrides, screen reader live announcements, and Web Speech API text-to-speech voice guidance.

UI/UX Architecture: Designed with clear section tabs, telemetry logs, and a dedicated emergency dispatch workflow.

### Challenges we ran into

Designing a responsive canvas-based indoor mapping system that visually demonstrates node-based routing and obstacle-bypassing in real-time.Structuring comprehensive local medical data specifically tailored to Gwinnett County infrastructure (Lawrenceville, Duluth, Snellville, Norcross, etc.).Ensuring the UI remained fully compliant with high-contrast, screen reader, and speech synthesis standards.

### Accomplishments that we're proud of

Successfully integrating a fully functional Ride Gwinnett paratransit and NEMT dispatch simulator with automated driver instructions.   Building 16+ real, verified Gwinnett healthcare facility entries complete with custom parking and entrance specifications.   Creating an inclusive, accessible user experience featuring live activity logging, high-contrast themes, and one-touch emergency hospital assist.   

### What we learned

The importance of micro-navigation details—such as door width, ramp incline angles, and elevator reliability—in physical medical accessibility.How to combine multiple civic services (public transit, hospital directories, and emergency helplines) into a single unified web application.

### What's next for "what should we make our team name"

Expanding the directory to cover more surrounding counties across Metro Atlanta.Integrating live API feeds from public transit authorities for real-time paratransit vehicle tracking.Partnering with local Gwinnett healthcare networks to crowdsource real-time accessibility status updates for facility elevators and ramps.

---

<a id="project-what-if-cgfxb1"></a>
## 16. What if?

- **Devpost:** [What if?](https://devpost.com/software/what-if-cgfxb1)
- **Crawl ID:** `what-if-cgfxb1`
- **Submitted to:** HackGwinnett 6.0
- **Built with:** accessibility, ai, dashboard, designsystem, frontend, hackathon, healthcare, healthtech, interactive, javascript, opensource, patientcare, react, responsive, simulation, socialgood, tailwindcss, ui/ux, vite

### Team

- [Lokaranjan Katakam Saravana](https://devpost.com/lokaranjanks1)
- [Sriram Kandanadan](https://devpost.com/kandanadansriram)

### Project links

- [drive.google.com/file/d/1tN0zTkXMILgs130ue1hWP-g94biLZkWS/view](https://drive.google.com/file/d/1tN0zTkXMILgs130ue1hWP-g94biLZkWS/view?usp=sharing)

### Technology references

- [javascript](https://devpost.com/software/built-with/javascript)
- [react](https://devpost.com/software/built-with/react)

### Project description

- Inspiration: Healthcare accessibility is often treated as a binary checklist rather than a nuanced reality, leaving patients vulnerable to unexpected obstacles like broken elevators or missing equipment.

- What it does: The platform empowers patients with an interactive Multiverse simulator for contingency planning, a digital Accessibility Passport for easy profile sharing, and a facility Reality Check for accommodation auditing.

- How we built it: It was developed using React, Vite, and Tailwind CSS, featuring a custom decision-tree traversal engine and native accessibility toggles like high-contrast mode and text-to-speech.

- Challenges & Learnings: Key challenges included balancing deep simulation workflows with a clean UI, teaching us that proactive contingency planning significantly reduces medical appointment anxiety.

- What's next: Future goals include building live hospital data integrations, expanding AI scenario personalization, and launching dedicated caregiver and provider portals.

---

<a id="project-safe-space-stories"></a>
## 17. Safe Space Stories

- **Devpost:** [Safe Space Stories](https://devpost.com/software/safe-space-stories)
- **Crawl ID:** `safe-space-stories`
- **Submitted to:** HackGwinnett 6.0
- **Built with:** googlesites

### Team

- [George Zhang](https://devpost.com/dream-techno999)

### Project links

- [sites.google.com/view/safespacestories/home](https://sites.google.com/view/safespacestories/home?authuser=0)

### Images

- [Image 1](https://d112y698adiu2z.cloudfront.net/photos/production/software_photos/005/765/292/datas/original.png)

### Project description

- Website front page to show users generalized examples

### Inspiration

Medical visits can be deeply overwhelming and unpredictable for neurodivergent individuals, frequently leading to intense anxiety and healthcare avoidance. While custom social stories are a proven clinical tool to ease this distress, creating them manually is time-consuming for families and caregivers. We wanted to bridge this gap by making cognitive accessibility effortless.

### What it does

Safe Space Stories is an AI-powered platform that instantly generates personalized, visual social stories and comics for medical procedures like bloodwork, MRIs, and vaccinations. By transforming fear-inducing unknowns into relatable scenarios it helps reduce waiting-room anxiety, restores dignity, and provides a reliable coping tool. It considers many factors when generating the stories that are created including color theory (maximizing comforting colors) and the understanding of the placebo effect where research showing the idea of a solution for a scary problem will decrease the level of stress and fear of a patient.

### How we built it

We designed and used Google Sites to make the website and took inspiration from current problems and research around medical anxiety.

### Challenges we ran into

We had limited technical ability so we needed to be creative and work around that challenge.

### Accomplishments that we're proud of

Creating a more tailored solution for neurodivergent people to help with their anxiety around the medical system.

### What we learned

How to create a website and clearly articulate a real life problem and our solution.

### What's next for Safe Space Stories

Implement and create an image generation that is tailored towards this project specifically and can help users with their fears.

---

<a id="project-carenori"></a>
## 18. CareNori

- **Devpost:** [CareNori](https://devpost.com/software/carenori)
- **Crawl ID:** `carenori`
- **Submitted to:** HackGwinnett 6.0
- **Built with:** api, coco-ssd, css, css3, github, gl, html5, javascript, maplibre, mediapipe, openfreemap, openstreetmap, react, speech, sqlite, tailwind, tensorflow.js, tesseract.js, typescript, vite, web

### Team

- [Giovanni Macli](https://devpost.com/maramelowmacli)
- [Angel Issac](https://devpost.com/angel-issac0990)

### Project links

- [github.com/ApoGamess/HackGwinnett6.0](https://github.com/ApoGamess/HackGwinnett6.0)

### Images

- [Image 1](https://d112y698adiu2z.cloudfront.net/photos/production/software_photos/005/765/127/datas/original.png)
- [Image 2](https://d112y698adiu2z.cloudfront.net/photos/production/software_photos/005/765/128/datas/original.png)
- [Image 3](https://d112y698adiu2z.cloudfront.net/photos/production/software_photos/005/765/129/datas/original.png)
- [Image 4](https://d112y698adiu2z.cloudfront.net/photos/production/software_photos/005/765/130/datas/original.png)
- [Image 5](https://d112y698adiu2z.cloudfront.net/photos/production/software_photos/005/765/131/datas/original.png)
- [Image 6](https://d112y698adiu2z.cloudfront.net/photos/production/software_photos/005/765/132/datas/original.png)

### Technology references

- [css](https://devpost.com/software/built-with/css)
- [css3](https://devpost.com/software/built-with/css3)
- [github](https://devpost.com/software/built-with/github)
- [html5](https://devpost.com/software/built-with/html5)
- [javascript](https://devpost.com/software/built-with/javascript)
- [openstreetmap](https://devpost.com/software/built-with/openstreetmap)
- [react](https://devpost.com/software/built-with/react)
- [sqlite](https://devpost.com/software/built-with/sqlite)
- [typescript](https://devpost.com/software/built-with/typescript)
- [web](https://devpost.com/software/built-with/web)

### Project description

CareNori — Find Care. Understand It. Be Heard.

### 💡 Inspiration

Accessing healthcare should not be more difficult because someone has a disability.

People with mobility, visual, hearing, or communication disabilities often face additional barriers when navigating hospitals, understanding medical documents, finding accessible entrances, or communicating with healthcare professionals.

We wanted to build something that goes beyond a traditional healthcare website.

That's why we created CareNori — an AI-powered healthcare accessibility companion designed to help people navigate medical environments with greater independence and confidence.

Our goal is simple: make healthcare more accessible, understandable, and inclusive for everyone.

### 🚀 What It Does

CareNori combines healthcare navigation, accessibility information, computer vision, and communication assistance into one connected experience.

Its core features include:

- Accessible Healthcare Navigation: Interactive maps that help users explore healthcare facilities and find information about wheelchair-accessible entrances, ramps, elevators, and other accommodations.

- AI Camera Assistance: Computer vision designed to recognize supported objects, identify people in view, and provide helpful descriptions of the user's surroundings.

- Smart Document Reader: Tools for reading signs and simplifying appointment information.

- Communication Assistant: Text-to-speech, customizable messages, and communication shortcuts for people who have difficulty speaking.

- Personalized Accessibility: Adjustable interfaces and accessibility preferences tailored to individual needs.

- Visit Preparation: A connected workspace for organizing appointment details, important questions, and accessibility requirements.

Rather than switching between multiple applications, users can access these capabilities in one place.

### 🛠️ How We Built It

We designed CareNori as a modern, browser-based application using technologies that support accessibility, interactive mapping, and artificial intelligence.

Our development approach combines:

- React and TypeScript for the application interface.

- Tailwind CSS for responsive and accessible design.

- MapLibre GL JS and OpenStreetMap for geographic visualization and accessibility-related location information.

- TensorFlow.js for browser-based computer vision.

- Tesseract.js for optical character recognition.

- Web Speech APIs for voice-based communication.

- Structured data for healthcare locations, accessibility features, and user preferences.

We focused on connecting these technologies into a single experience rather than developing isolated tools.

For the hackathon, our approach prioritizes a functional prototype with clearly identified demonstration data and opportunities for future integrations.

### 🧩 Challenges We Faced

One of our biggest challenges was combining several complex technologies while keeping the application simple and accessible.

Building useful navigation: Traditional maps do not always provide enough information about accessible entrances, elevators, or indoor routes.

Integrating computer vision: Camera-based assistance requires careful attention to model accuracy, device performance, and real-world limitations.

Designing for different disabilities: An interface that works well for one user may create barriers for another. We had to consider different ways of navigating, reading, and communicating.

Working with incomplete data: Accessibility information is not always available or verified. We wanted to avoid presenting uncertain information as fact.

These challenges helped us understand that accessibility requires more than adding features. It requires designing the entire experience around people's needs.

### 📚 What We Learned

Building CareNori taught us how artificial intelligence, mapping technologies, and accessible interface design can work together to address real-world challenges.

We learned that technology should support independence without creating unnecessary complexity.

We also learned the importance of communicating technical limitations clearly, especially when users may depend on information about physical accessibility.

Most importantly, we discovered that the value of technology is not only what it can do, but how effectively it helps people.

### 🌎 What's Next for CareNori?

Our long-term vision is to make CareNori a comprehensive healthcare accessibility companion.

Future development could include:

- More detailed accessible indoor navigation.

- Improved computer vision and environmental descriptions.

- Expanded healthcare accessibility datasets.

- Multilingual communication assistance.

- Partnerships with healthcare facilities.

- More personalized accessibility tools.

We envision a future where navigating a hospital, understanding healthcare information, and communicating with medical professionals are easier for everyone.

CareNori isn't about replacing healthcare professionals. It's about removing barriers between people and the care they need.

### CareNori — Find Care. Understand It. Be Heard.

*No details provided in the crawl.*

---

<a id="project-medical-div"></a>
## 19. Medical Div

- **Devpost:** [Medical Div](https://devpost.com/software/medical-div)
- **Crawl ID:** `medical-div`
- **Submitted to:** HackGwinnett 6.0
- **Built with:** github, react, typescript

### Team

- [Hacke025 Patel](https://devpost.com/Hacke025)

### Project links

- [github.com/Hacke025/Medical-Div/tree/main](https://github.com/Hacke025/Medical-Div/tree/main)
- [hacke025.github.io/Medical-Div](https://hacke025.github.io/Medical-Div/)
- [drive.google.com/file/d/1iD7MTnW8SOWG-3x38PCnxSJ6sikYUMbD/view](https://drive.google.com/file/d/1iD7MTnW8SOWG-3x38PCnxSJ6sikYUMbD/view?usp=drive_link)
- [drive.google.com/file/d/1fSkIVbk7n_vyBPH-kvGhzdXDCYhcTTjr/view](https://drive.google.com/file/d/1fSkIVbk7n_vyBPH-kvGhzdXDCYhcTTjr/view?usp=drivesdk)
- [youtu.be/F6zv-4PIJXA](https://youtu.be/F6zv-4PIJXA?si=sPLAg7N0z03XBE8t)

### Technology references

- [github](https://devpost.com/software/built-with/github)
- [react](https://devpost.com/software/built-with/react)
- [typescript](https://devpost.com/software/built-with/typescript)

### Project description

Careway — Healthcare, Made Clearer

Making healthcare easier to understand, navigate, and access for everyone.

### Inspiration

Healthcare can be difficult to navigate. Between complicated terminology, confusing forms, appointment instructions, insurance information, and digital healthcare systems, even simple tasks can become overwhelming.

These barriers can be especially challenging for people with disabilities or different accessibility needs. However, difficulty navigating healthcare is not limited to one group. Anyone can struggle to understand an unfamiliar medical term, follow a long appointment notice, or figure out what a form is asking.

I wanted to explore how technology and thoughtful design could make healthcare information easier to understand and healthcare experiences more accessible. This led to Careway: a tool designed around the idea that accessibility should be built into the experience from the beginning, rather than treated as an optional extra.

### What It Does

Careway is an accessible healthcare navigation prototype that helps users understand information, prepare for appointments, and personalize their experience.

Some of its main features include:

- Reading Companion: Organizes long healthcare messages into smaller sections and highlights possible dates, times, costs, phone numbers, and action words.

- Document Reader: Allows users to upload text and Markdown documents, break them into readable sections, and listen to the content.

- Accessibility Settings: Offers adjustable text size, high contrast, dark mode, increased text spacing, a dyslexia-friendly font option, and reduced motion.

- Voice Assistant: Provides voice commands and spoken page content to make navigation easier.

- Healthcare Glossary: Explains common healthcare and insurance terminology in simpler language.

- Careway Navigator: Provides plain-language explanations and examples for confusing healthcare form fields.

- Access Passport: Applies saved accessibility preferences to the Careway experience.

- Barrier Scanner: Checks the page for several common accessibility markup issues.

- Appointment Question Builder: Helps users create questions to bring to an appointment.

- Appointment Checklist and Pack: Combines preparation tasks, questions, and access preferences into a printable summary.

- Language Support: Provides English and Spanish sample phrases and a bilingual appointment preparation sheet.

### How I Built It

With the help of AI,

I built Careway as a web application using React and TypeScript. Vite provides the development and build environment, while CSS is used to create the responsive interface and accessibility-related styling.

I used Lucide React for interface icons and built several features around browser capabilities, including text-to-speech, speech recognition, local storage, and clipboard functionality.

The project is hosted through GitHub Pages, with GitHub Actions automatically building and deploying updates when changes are pushed to the repository.

The current prototype primarily runs in the user's browser. It does not require a separate application server, database, or connected generative AI service.

### Challenges I Faced

One of the biggest challenges was designing accessibility features that could work together without making the application feel complicated. Different users may need different combinations of text, visual, movement, communication, or navigation adjustments.

Another challenge was making Careway useful to everyone rather than designing it exclusively around disability-specific features. I wanted users to be able to arrive with a simple problem, such as understanding a healthcare message, and find help without needing to identify themselves or disclose personal information.

I also had to consider privacy. Healthcare information can be sensitive, so I designed the prototype to avoid sending user-entered information to a healthcare provider or a Careway backend. The application uses browser storage for demo preferences and clearly communicates that users should not enter real medical or identifying information.

Finally, I had to work within the limitations of browser technology. Speech recognition support varies between browsers, and the current document reader supports text and Markdown files rather than PDFs or scanned documents. The language feature also provides prepared English and Spanish phrases rather than live translation.

### What I Learned

Building Careway helped me understand that accessibility is not just about adding a few settings. It affects how an entire application is organized, how information is presented, how controls behave, and how users move through an experience.

I also learned how to combine multiple browser technologies into a cohesive application, build reusable interactive components, and deploy a project through GitHub Actions and GitHub Pages.

Most importantly, I learned that a useful accessibility tool does not have to make users feel different. It should simply make the experience work better for them.

### What's Next

Some possible future improvements include:

- Expanding language support and translating more of the interface.

- Adding PDF and scanned-document reading capabilities.

- Improving compatibility with screen readers and assistive technologies.

- Exploring optional AI-powered explanations with clear consent and privacy safeguards.

- Developing a browser extension to help identify accessibility barriers on external healthcare websites.

- Testing the application with people who have different accessibility needs.

### Important Note

Careway is an early-stage demonstration, not a medical service or patient portal. It does not provide medical advice, diagnosis, or treatment recommendations, and it does not connect to healthcare providers. Its language support is limited to prepared English and Spanish content, not live interpretation. Users should not enter real medical or identifying information into the prototype.

---

<a id="project-accesscare"></a>
## 20. AccessCare

- **Devpost:** [AccessCare](https://devpost.com/software/accesscare)
- **Crawl ID:** `accesscare`
- **Submitted to:** HackGwinnett 6.0
- **Built with:** css, html, java, react, tailwind, typscript

### Team

- [Sriram V](https://devpost.com/sriram-vakkalanka)
- [Sri Raghavendra Kesava](https://devpost.com/raghavkesava2024)
- [Rishi V](https://devpost.com/rishi-vutukuri)

### Project links

- [github.com/Rvshark-control/AccessReady-HackGwinnett6/tree/main](https://github.com/Rvshark-control/AccessReady-HackGwinnett6/tree/main)

### Images

- [Image 1](https://d112y698adiu2z.cloudfront.net/photos/production/software_photos/005/765/272/datas/original.png)
- [Image 2](https://d112y698adiu2z.cloudfront.net/photos/production/software_photos/005/765/273/datas/original.png)
- [Image 3](https://d112y698adiu2z.cloudfront.net/photos/production/software_photos/005/765/275/datas/original.png)
- [Image 4](https://d112y698adiu2z.cloudfront.net/photos/production/software_photos/005/765/274/datas/original.png)
- [Image 5](https://d112y698adiu2z.cloudfront.net/photos/production/software_photos/005/765/276/datas/original.png)
- [Image 6](https://d112y698adiu2z.cloudfront.net/photos/production/software_photos/005/765/277/datas/original.png)

### Technology references

- [css](https://devpost.com/software/built-with/css)
- [html](https://devpost.com/software/built-with/html)
- [java](https://devpost.com/software/built-with/java)
- [react](https://devpost.com/software/built-with/react)

### Project description

### Inspiration

Navigating healthcare is already challenging, but for individuals with specialized physical, sensory, or mobility needs, finding a facility that actually accommodates them is a constant hurdle. Patients frequently arrive at appointments only to encounter unexpected physical barriers, broken elevator access, or a lack of specialized equipment. We created AccessReady to remove this dangerous guessing game from medical navigation, giving patients full transparency so they can seek care with confidence and peace of mind.

### What it does

AccessReady is a specialized healthcare accessibility matching web app that instantly connects individuals with medical facilities equipped for their precise accommodation needs. Using a custom compatibility algorithm, the app scores and matches facilities based on physical mobility support, sensory accommodations, and specialized medical equipment. Features include verified facility breakdowns, barrier indicators, interactive search filtering, and clean routing—all presented through a responsive UI.

### How we built it

The frontend was engineered with Next.js 16 (using Turbopack) and Tailwind CSS, styled in a dark-mode Halloween visual palette (Midnight Charcoal background, Electric Pumpkin Orange, Toxic Purple, and Eerie Slime Green). We designed a "liquid glass" glassmorphism aesthetic using frosted semi-transparent cards (backdrop-blur-md), smooth scroll behavior, and fluid micro-animations. On the backend, we structured matching workflows to evaluate user accessibility preferences against facility data models in real time.

### Challenges we ran into

Early in the hackathon, we hit significant hurdles with styling setups, broken asset paths, uncompiled layout directives, and severe Git merge conflicts across entire files in README.md. We solved this by pivoting to a fresh repository, establishing parallel feature branches (claude-frontend-ui for frontend layout work and codex-backend for backend logic), and systematically re-linking our global CSS imports to ensure clean, error-free builds.

### Accomplishments that we're proud of

We are proud to have delivered a fully responsive, visually distinct "liquid glass" dark mode UI without sacrificing web accessibility or readability. Overcoming team repo conflicts to establish a smooth multi-branch workflow—and taking the application from an unstyled prototype to a polished, fully functioning full-stack demo—was a major milestone for our team.

### What we learned

Working on AccessReady reinforced the power of disciplined Git branch management, clean project folder structuring, and fast prototyping with modern frontend tooling. We deepened our practical knowledge of Next.js Turbopack workflows, advanced Tailwind CSS styling techniques, and accessibility-first UI design patterns.

### What's next for AccessCare

Looking ahead, we aim to expand our database through direct healthcare provider API integrations and community-driven accessibility reviews. Future planned features include real-time facility status updates (e.g., live elevator outage alerts), multi-language voice navigation, and direct appointment booking integrations to establish AccessReady as a comprehensive standard for barrier-free healthcare access.

---

<a id="project-medicrate"></a>
## 21. Medicrate

- **Devpost:** [Medicrate](https://devpost.com/software/medicrate)
- **Crawl ID:** `medicrate`
- **Submitted to:** HackGwinnett 6.0
- **Built with:** api, css, deep, flask, git, google, gps, html, javascript, json, links, maps, places, platform, python, python-dotenv, requests, rest, routes, uber

### Team

- [Sarvesh Vijayamanikandan](https://devpost.com/sv47-gsmst)
- [Jaimin Suh](https://devpost.com/jaimin-mason-suh)
- [Eshaan Shah](https://devpost.com/shaheshaan20)

### Project links

- [github.com/sv47-gsmst/Medicrate](https://github.com/sv47-gsmst/Medicrate)

### Technology references

- [css](https://devpost.com/software/built-with/css)
- [flask](https://devpost.com/software/built-with/flask)
- [git](https://devpost.com/software/built-with/git)
- [google--2](https://devpost.com/software/built-with/google--2)
- [gps](https://devpost.com/software/built-with/gps)
- [html](https://devpost.com/software/built-with/html)
- [javascript](https://devpost.com/software/built-with/javascript)
- [json](https://devpost.com/software/built-with/json)
- [python](https://devpost.com/software/built-with/python)
- [requests](https://devpost.com/software/built-with/requests)
- [uber](https://devpost.com/software/built-with/uber)

### Project description

Medicrate: Smart Emergency Healthcare Routing

### Inspiration

When facing a sudden medical emergency or requiring specialized treatment, people almost always make a panicked decision: they open a navigation app and drive to the nearest hospital. However, proximity does not equal suitability. The nearest facility may have a 4-hour emergency room wait time, lack trauma care capabilities, or rank poorly for the specific condition at hand.

While modern technology effortlessly optimizes routes for food delivery or ride-shares, critical healthcare navigation remains fragmented and guesswork-driven. We built Medicrate to bridge this gap—creating a smart, data-driven matching system that directs patients not just to the closest hospital, but to the right hospital in the fastest effective time.

### What It Does

Medicrate is an intelligent healthcare dispatch and navigation web application that eliminates friction during medical emergencies and specialized care searches.

- Condition-Based Hospital Matching: Users enter their medical situation or symptom, and Medicrate instantly filters facilities based on specialization, survival rate, and equipment readiness.

- Dynamic Travel & Wait-Time Optimization: Computes total transit and queue time to minimize time-to-care.

- Turn-by-Turn Navigation: Integrates directly with Google Maps to provide optimized driving routes and seamless step-by-step guidance.

- Live ER Analytics: Tracks real-time emergency department wait times and capacity status.

### Mathematical Foundation

To ensure patients reach the optimal facility, Medicrate evaluates every nearby hospital $i$ using a weighted utility scoring function $U_i$:

$$U_i = w_s \cdot S_i + w_q \cdot Q_i - w_t \cdot E_i$$

Where:

- $S_i \in [0, 100]$ is the hospital's specialization score for the target condition.

- $Q_i \in [0, 100]$ is the clinical quality and outcome rating.

- $E_i$ is the Effective Delay Time in minutes, calculated as:

$$E_i = T_{\text{travel}}(i) + T_{\text{wait}}(i)$$

- $T_{\text{travel}}(i)$ represents real-time driving duration from Google Maps API.

- $T_{\text{wait}}(i)$ is the current estimated ER wait time.

- $w_s, w_q, w_t$ are normalized weights ($\sum w = 1$) dynamically adjusted based on severity.

For critical emergencies, $w_t$ increases rapidly to prioritize minimum $E_i$, whereas for specialized scheduled care, $w_s$ and $w_q$ take precedence.

### How We Built It

- Frontend: Built with React and Tailwind CSS to deliver an ultra-responsive, accessible interface designed for rapid decision-making under stress.

- Backend: Powered by Node.js and Express RESTful endpoints that handle algorithmic hospital filtering and weighted scoring.

- Mapping Integration: Embedded Google Maps JavaScript API, Directions API, and Distance Matrix API for real-time traffic updates, distance calculations, and interactive map displays.

- Data Layer: Normalized hospital metrics, specialty ratings, and emergency department queue data stored in a relational PostgreSQL database.

### Challenges We Ran Into

- Data Standardization: Aggregating data across disjointed sources (CMS ratings, specialty certifications, and real-time ER tracking) required extensive schema mapping and data sanitization.

- Routing Latency: Calculating real-time traffic for multiple candidate hospitals simultaneously posed speed challenges. We optimized spatial indexing to query only facilities within a dynamic bounding radius before making API distance calls.

- High-Stress UX: Designing an interface that provides maximum information with minimal cognitive load during panic situations required stripping away extraneous UI elements and focusing on clear visual hierarchy.

### Accomplishments That We're Proud Of

- Successfully merging real-time geographic routing with clinical outcome data into a single unified recommendation engine.

- Building a working prototype that calculates the mathematically optimal care destination in under 2 seconds.

- Crafting a fully responsive, high-contrast user interface accessible across all mobile and desktop devices.

### What We Learned

- Geospatial Optimization: Gained deep experience utilizing Google Maps API services for multi-point distance calculations and live route rendering.

- Healthcare Logistics: Developed a clear understanding of clinical capacity metrics, triage dynamics, and emergency dispatch variables.

- User-Centric Engineering: Reinforced the principle that in emergency-focused applications, speed and simplicity in design are life-saving features.

### What's Next for Medicrate

- Live Hospital Telemetry: Partnering with regional hospital networks to ingest direct automated feeds for real-time bed availability and ER wait queues.

- Insurance Matching: Incorporating dynamic insurance network filters to ensure patients avoid out-of-network surprise billing.

- Voice-Activated Triage: Integrating hands-free voice commands so drivers or panicked patients can navigate to care safely without typing.

---

<a id="project-carefit"></a>
## 22. CareFit

- **Devpost:** [CareFit](https://devpost.com/software/carefit)
- **Crawl ID:** `carefit`
- **Submitted to:** HackGwinnett 6.0
- **Built with:** claude, codex, css3, git, html5, leatlet, node.js, ollama, pwa, qwen2.5, react, typescript, vite

### Team

- [Loukik Garine](https://devpost.com/Bubby3999)

### Project links

- [github.com/Bubby3999/Skill-Hack-o-ton](https://github.com/Bubby3999/Skill-Hack-o-ton)

### Technology references

- [css3](https://devpost.com/software/built-with/css3)
- [git](https://devpost.com/software/built-with/git)
- [html5](https://devpost.com/software/built-with/html5)
- [node-js](https://devpost.com/software/built-with/node-js)
- [react](https://devpost.com/software/built-with/react)
- [typescript](https://devpost.com/software/built-with/typescript)

### Project description

### Inspiration

Many wheelchair users go years without being weighed or examined on a table, because their clinic has no accessible scale or exam table. Deaf patients arrive to find no interpreter booked. Autistic patients walk into loud, bright waiting rooms with no warning. In 2026, new federal rules (HHS Section 504 and DOJ ADA Title II) started requiring most providers to have accessible exam tables and scales. Patients still have no way to see which clinics do. We built CareFit so disabled patients can find a doctor who can examine them before they show up.

### What it does

CareFit is a phone-first web app that matches a patient's access needs to clinics that meet them.
Profile: you choose your access needs across mobility, communication, sensory/cognitive, and other. Each one is marked required or nice to have. You also set your location (GPS or ZIP code) and a search radius. Everything stays on your phone.
Search: filter by type of care, distance, and needs, or ask the AI assistant in plain language, e.g. "OB-GYN within 15 miles who can weigh me seated."
Match: each clinic gets a fit score with reasons in plain text, e.g. has: wheelchair scale · missing: ASL interpreter · unknown: patient lift. Results appear as a list or on a map.
Act: open a clinic's details, then create an accommodation request letter that cites Section 504 and the ADA. You can copy, share, email, or print it.
The demo uses about 20 fictional Oakland clinics, labeled Demo data. Public data on clinic equipment doesn't exist, and that gap is the problem CareFit addresses.

### How we built it

We spent the first phase defining the problem, the users, and the features. Then we designed mockups for every screen and checked them for color contrast. Next came a step-by-step build plan. Claude Opus 5.5 helped us plan, and Claude Sonnet 5.5 agents wrote the code in parallel, one per group of screens. We reviewed and tested each part. The app uses Vite, React, and TypeScript, with Leaflet and OpenStreetMap for the map. A small Node server connects the assistant to a local Ollama model, so no messages go to an AI company. We target WCAG 2.2 AA accessibility and test with Playwright and axe.

### Challenges we ran into

We spent more time than planned defining the problem and deciding what to build during the hackathon.  We had to build with clearly labeled demo data rather than make claims about real clinics and it took us a bit time and planning to confirm our mockup designs before we built the official submission.

### Accomplishments that we're proud of

We built a working platform for a real problem: disabled patients often can't tell whether a clinic has the equipment or support they need until they arrive. CareFit matches each user's access needs, such as an accessible exam table, an ASL interpreter or a quiet room, against a library of clinics, shows the matches on a map and drafts an accommodation request letter. We shipped it as a full-stack, phone-first web app with an AI assistant that runs on a local model, so users' data isn't sent to an outside AI company. We also used Claude to help shape the architecture and to plan how users would find and use these tools.

### What we learned

We learned to stay calm and focused under a tight deadline while keeping the people we were building for at the center. Our process worked best in this order:

Brainstorm the idea as a team.
Research the problem and find real examples, such as wheelchair users who go years without being weighed because their clinic has no accessible scale.
Review our codebase, then hold focused sessions with Claude on specific questions and code snippets we weren't sure about.
Asking narrow, specific questions gave us much better results than asking broad ones.

### What's next for CareFit

More data sources: connect APIs and public provider directories to make clinic information more complete and accurate.
Community reports: let patients report when a clinic's accessibility doesn't match its listing.
Real clinic data: replace our demo clinics with verified listings, starting in one city.

---

<a id="project-carebloom-2tvazc"></a>
## 23. CareBloom

- **Devpost:** [CareBloom](https://devpost.com/software/carebloom-2tvazc)
- **Crawl ID:** `carebloom-2tvazc`
- **Submitted to:** HackGwinnett 6.0
- **Built with:** vercel

### Team

- [Aaron Wang](https://devpost.com/bigtinytacosjr7892)
- [Michael Ayers](https://devpost.com/xcrept0001)

### Project links

- [nextjs-boilerplate-green-nine-71.vercel.app](https://nextjs-boilerplate-green-nine-71.vercel.app/)

### Images

- [Image 1](https://d112y698adiu2z.cloudfront.net/photos/production/software_photos/005/765/334/datas/original.png)
- [Image 2](https://d112y698adiu2z.cloudfront.net/photos/production/software_photos/005/765/342/datas/original.png)

### Project description

- Dcotor side UI

- Doctor side UI

### Inspiration

My grandmother did not get the proper medical care she needed for her stomach disease. She was not aware of the counter measures to take because the doctors did not explicitly tell her. This made her bedridden for over a month before she passed peacefully in her sleep. Because of this lack of awareness on what to do, Michael and I made this website to counteract this lack of information and help guide patients with plans and goals to achieve that will help them with their issues.

### What it does

CareBloom helps doctors explore patient records and helps patients understand their care through AI chat, personalized daily tasks, and XP rewards.

### How we built it

We used Next.js to create separate doctor and patient dashboards connected through shared sample patient data. Used Claude + Vercel to build out the website

### Challenges we ran into

We had to make medical information useful for doctors while keeping it simple for patients, all within a short build time.

### Accomplishments that we're proud of

We connected medical records to daily goals, giving patients something useful to act on after an appointment.

### What we learned

Making healthcare accessible means considering how people understand information and what they can realistically do each day.

### What's next for CareBloom

We want feedback from disabled users and doctors, better accessibility support, and optional Apple Watch and Strava connections.

---

<a id="project-sms-shield-gtks0o"></a>
## 24. SMS Shield

- **Devpost:** [SMS Shield](https://devpost.com/software/sms-shield-gtks0o)
- **Crawl ID:** `sms-shield-gtks0o`
- **Submitted to:** DSH Hacks V2 ($100k+ in prizes!), HackGwinnett 6.0, Pumpkin Playground, STEM2Connect AI Hackathon
- **Built with:** aria, css3, elevenlabs, elevenlabs-speech-to-text, elevenlabs-text-to-speech, express.js, getusermedia, git, github, google-fonts, gpt-oss-120b, groq, html5, intersectionobserver, javascript, mediapipe, mediarecorder-api, node.js, qwen, svg, vercel, wcag, web-speech-api, webgl

### Team

- [Shaina Mereddy](https://devpost.com/shainamereddy)
- [Manya Mereddy](https://devpost.com/manyamereddy)
- [sujaygodala3-hub Godala](https://devpost.com/sujaygodala3-hub)

### Project links

- [github.com/sujaygodala3-hub/sms-shield](https://github.com/sujaygodala3-hub/sms-shield)
- [sms-shield-ten.vercel.app](https://sms-shield-ten.vercel.app/)

### Images

- [Image 1](https://d112y698adiu2z.cloudfront.net/photos/production/software_photos/005/765/124/datas/original.png)
- [Image 2](https://d112y698adiu2z.cloudfront.net/photos/production/software_photos/005/765/133/datas/original.png)
- [Image 3](https://d112y698adiu2z.cloudfront.net/photos/production/software_photos/005/765/158/datas/original.png)
- [Image 4](https://d112y698adiu2z.cloudfront.net/photos/production/software_photos/005/765/159/datas/original.png)
- [Image 5](https://d112y698adiu2z.cloudfront.net/photos/production/software_photos/005/765/210/datas/original.png)
- [Image 6](https://d112y698adiu2z.cloudfront.net/photos/production/software_photos/005/765/160/datas/original.png)
- [Image 7](https://d112y698adiu2z.cloudfront.net/photos/production/software_photos/005/765/162/datas/original.png)
- [Image 8](https://d112y698adiu2z.cloudfront.net/photos/production/software_photos/005/765/167/datas/original.png)
- [Image 9](https://d112y698adiu2z.cloudfront.net/photos/production/software_photos/005/765/178/datas/original.png)
- [Image 10](https://d112y698adiu2z.cloudfront.net/photos/production/software_photos/005/765/181/datas/original.png)
- [Image 11](https://d112y698adiu2z.cloudfront.net/photos/production/software_photos/005/765/182/datas/original.png)
- [Image 12](https://d112y698adiu2z.cloudfront.net/photos/production/software_photos/005/765/185/datas/original.png)
- [Image 13](https://d112y698adiu2z.cloudfront.net/photos/production/software_photos/005/765/188/datas/original.png)
- [Image 14](https://d112y698adiu2z.cloudfront.net/photos/production/software_photos/005/765/192/datas/original.png)

### Technology references

- [aria](https://devpost.com/software/built-with/aria)
- [css3](https://devpost.com/software/built-with/css3)
- [express-js](https://devpost.com/software/built-with/express-js)
- [git](https://devpost.com/software/built-with/git)
- [github](https://devpost.com/software/built-with/github)
- [google-fonts](https://devpost.com/software/built-with/google-fonts)
- [groq](https://devpost.com/software/built-with/groq)
- [html5](https://devpost.com/software/built-with/html5)
- [javascript](https://devpost.com/software/built-with/javascript)
- [node-js](https://devpost.com/software/built-with/node-js)
- [webgl](https://devpost.com/software/built-with/webgl)

### Project description

- Enter Screen

- Page to choose disability option

- Home Page

- Display Options

- Tools Section

- FAQ Section

- Photo Check 1/2

- Photo Check 2/2

- Symptoms Page

- Bill Check 1/2

- Bill Check 2/2

- Cost Page

- Medication Page

- Rights & Letters Page

### Inspiration

Healthcare should be accessible to everyone, yet millions of Americans face barriers when seeking medical assistance. According to the CDC, over 70 million American adults live with a disability, while medical debt continues to create financial challenges for families nationwide. We realized that individuals who are deaf, blind, nonspeaking, or have limited mobility may face additional difficulties communicating symptoms, understanding treatment options, and advocating for their legal rights.

This inspired us to create SMS Shield, an AI-powered platform designed to bridge the gap between healthcare accessibility, affordability, and patient empowerment. Our goal was to ensure that no disability, financial barrier, or lack of legal knowledge prevents patients from understanding their healthcare options.

### What it does

SMS Shield combines medical guidance, financial assistance, and patient-rights education into one accessible platform.

Users can describe symptoms through voice or text, upload photographs of visible medical concerns for AI-assisted analysis, and explore potential treatment options. Specialized accessibility modes accommodate individuals with visual, hearing, speech, and mobility disabilities, including hands-free facial navigation, spoken guidance, and customizable display settings.

Beyond symptom analysis, SMS Shield helps patients identify potentially unlawful medical charges, explore hospital financial assistance, compare estimated treatment and medication costs, and understand protections under laws such as the ADA, No Surprises Act, and Section 504 of the Rehabilitation Act.

Our personalized letter generator also helps users prepare medical billing disputes, insurance appeals, and disability accommodation requests.

### How we built it

We built SMS Shield with plain HTML, CSS and JavaScript and no framework, so every page loads fast even on an old phone. We designed for accessibility first. Every screen works with just a keyboard, screen readers get proper labels, and there are options for high contrast, larger text and a calm mode with no motion.
A small Node.js and Express server sits behind the site so our API keys never reach the browser. If any service goes down, the site falls back to built-in answers or the browser’s own voice instead of breaking. It’s deployed on Vercel.
Groq powers our chatbot and photo check. The prompts make sure the AI always says “could be,” never diagnoses, and flags when to get urgent care. ElevenLabs gives the site one calm voice that reads everything aloud, and it powers a microphone on every text box. Hands-free mode uses MediaPipe face tracking right in the browser, so you can move around by turning your head, and the camera feed never leaves your device.
The heart of the project is our legal layer. It’s one shared file that both the site and the chatbot use, covering the ADA, Section 504, Section 1557, free interpreters, service animals, surprise-bill protections, charity care and insurance appeals. Every rule is in plain words with a real citation, and anything we couldn’t confirm is labeled a general principle. It also fills in six ready-to-send letters with the user’s details.
We’re proudest of the first screen. Since we can’t know who’s visiting, each option lights up and is read aloud in turn, and you just press space or tap anywhere when yours comes up. Someone who can’t see, hear or speak can get in on their own. Photos and recordings are never saved, and the whole design is built around our logo’s pinks and reds.

### Challenges we ran into

One of our biggest challenges was designing a platform that genuinely addresses different disabilities rather than offering a single accessibility solution. Features that benefit blind users may not serve deaf or nonspeaking individuals, requiring us to rethink how users interact with every part of the website.

Another challenge involved translating complex healthcare laws into understandable, situation-specific guidance. Medical billing protections vary depending on insurance coverage, hospital classification, financial circumstances, and other factors. We needed to structure our system to identify potentially relevant rights without presenting uncertain results as guaranteed legal conclusions.

We also had to balance AI functionality with medical safety, accessibility, privacy, and an intuitive user experience.

### Accomplishments that we're proud of

Our proudest accomplishment is transforming SMS Shield from a simple medical billing and symptom-checking tool into an inclusive, AI healthcare platform which was designed to empower individuals with disabilities. We developed multiple accessibility modes, including voice assistance for visually impaired users, text-based communication for deaf and nonspeaking individuals, and hands-free facial navigation for people with limited mobility.

We're especially proud of integrating medical guidance, financial assistance, and legal protections into one connected experience. Rather than only listing various healthcare laws, SMS Shield helps patients identify protections relevant to their circumstances and generate personalized dispute letters, insurance appeals, and disability accommodation requests.

Another major achievement was implementing AI photo analysis, symptom checking, and interactive cost comparisons while maintaining an accessible, user-friendly interface.

Above all, we're proud that SMS Shield addresses a meaningful real-world challenge: making healthcare information more accessible, affordable, and actionable for people who are often overlooked by traditional healthcare systems. Our greatest achievemen is the potential it has to help patients confidently advocate for their health, finances, and rights.

### What we learned

Developing SMS Shield taught us that innovation is not simply about creating advanced technology, but about making that technology genuinely useful and accessible to the people who need it most.

We strengthened our understanding of AI integration, frontend and backend development, conditional programming, accessibility-centered design, and healthcare regulations.

Most importantly, we learned how interconnected medical accessibility and financial security can be. Understanding a diagnosis is only one part of navigating healthcare; patients must also understand their treatment options, expenses, and legal protections.

SMS Shield represents our vision of a healthcare experience where patients are empowered not only to seek care, but also to understand their rights and confidently advocate for themselves.

### What's next for SMS Shield

Our next goal is to commercialize SMS Shield and transform it into a widely accessible healthcare technology platform that empowers individuals both inside and outside traditional medical settings.

We plan to integrate more precise medical technologies, including digital microscopes, advanced imaging systems, and AI-powered diagnostic support, allowing users to capture and analyze medical concerns in greater detail. By combining accessible software with innovative medical hardware, we hope to expand SMS Shield's capabilities beyond basic symptom analysis and provide more reliable information to patients who may face barriers accessing traditional healthcare facilities.

Additionally, we aim to develop SMS Shield into a user-friendly mobile application, making its accessibility features, medical guidance, financial assistance tools, and patient-rights resources more convenient to use anywhere, at any time.

We also envision collaborating with hospitals, healthcare professionals, and medical technology companies to improve accuracy, validate our technology, and expand its reach.

Ultimately, our vision is to make SMS Shield a commercially scalable, affordable, and inclusive healthcare solution that bridges the gap between advanced medical technology and everyday patients, regardless of disability, financial background, or access to healthcare facilities.

---

<a id="project-carebridge-504tgi"></a>
## 25. CareBridge

- **Devpost:** [CareBridge](https://devpost.com/software/carebridge-504tgi)
- **Crawl ID:** `carebridge-504tgi`
- **Submitted to:** HackGwinnett 6.0
- **Built with:** base44, geminiai

### Team

- [GSMST TSA](https://devpost.com/gsmst-ga-tsa)

### Project links

- [poised-bridge-access-flow.base44.app](https://poised-bridge-access-flow.base44.app/)

### Images

- [Image 1](https://d112y698adiu2z.cloudfront.net/photos/production/software_photos/005/764/523/datas/original.jpg)
- [Image 2](https://d112y698adiu2z.cloudfront.net/photos/production/software_photos/005/764/526/datas/original.jpg)
- [Image 3](https://d112y698adiu2z.cloudfront.net/photos/production/software_photos/005/764/525/datas/original.jpg)
- [Image 4](https://d112y698adiu2z.cloudfront.net/photos/production/software_photos/005/764/522/datas/original.jpg)
- [Image 5](https://d112y698adiu2z.cloudfront.net/photos/production/software_photos/005/764/527/datas/original.jpg)
- [Image 6](https://d112y698adiu2z.cloudfront.net/photos/production/software_photos/005/764/519/datas/original.jpg)
- [Image 7](https://d112y698adiu2z.cloudfront.net/photos/production/software_photos/005/764/520/datas/original.jpg)
- [Image 8](https://d112y698adiu2z.cloudfront.net/photos/production/software_photos/005/764/521/datas/original.jpg)
- [Image 9](https://d112y698adiu2z.cloudfront.net/photos/production/software_photos/005/764/518/datas/original.jpg)
- [Image 10](https://d112y698adiu2z.cloudfront.net/photos/production/software_photos/005/764/524/datas/original.jpg)

### Project description

- Developer Screen

- Patient Landing Screen

- Patient Request Option

- Patient Request Option

- Patient Request Option

- Patient Request Option

- Patient Request Option

- Patient Request Option

- Medical Staff Rating Option

- Staff Dashboard to View all Patient Requests

### Inspiration

The traditional hospital call button is a one-size-fits-all tool that fails both the most vulnerable patients and the medical supply chain. For non-verbal, neurodivergent, or physically disabled patients, pressing a button just summons a nurse to ask a question the patient might not be able to easily answer. Meanwhile, nurses spend a massive portion of their shifts playing "hide and seek" with medical equipment across the hospital. We realized that by giving patients an accessible voice, we could simultaneously solve the "last mile" problem of hospital inventory tracking. The inspiration for CareBridge came from wanting to empower patients with dignity while turning unpredictable equipment requests into actionable, tracked supply chain data.

### What it does

CareBridge is a zero-login Progressive Web App (PWA) accessed via a bedside QR code. For the patient, it acts as an Augmentative and Alternative Communication (AAC) device. Using massive touch targets and an intuitive icon grid, patients can specifically request what they need—whether that's pain medication, a bathroom trip, or physical equipment like a bariatric adapter, slide board, or sensory blanket.

Under the hood, CareBridge acts as a smart supply chain router. If a patient requests a clinical task (e.g., "Bathroom"), it routes to the nursing station. If they request a physical item (e.g., "Slide Board"), the request bypasses nursing entirely and routes directly to Central Supply. Once the supply tech approves the dispatch, the item is automatically decremented from the hospital's live inventory, providing real-time tracking and preventing misplaced stock.

### How we built it

We built the MVP as a Progressive Web App using HTML, Tailwind CSS, and vanilla JavaScript to ensure it was lightweight and universally compatible with any hospital tablet or phone. We utilized the Web Speech API to provide auditory confirmation for visually impaired users. To move away from cold, sterile hospital interfaces, we designed the frontend using neon, 3D cartoon, and Pixar-style aesthetics; this artistic direction naturally provided the high contrast and bold visual hierarchy required for WCAG compliance while making the experience feel warm and engaging for the user. We structured our mock backend using a JSON database schema to handle the dual-routing logic between the active_requests queue and the inventory decrementing functions.

### Challenges we ran into

Designing for extreme accessibility was our biggest hurdle. We had to ensure the app was usable by patients with severe motor tremors, which required us to engineer a custom JavaScript "debounce" function to prevent accidental multi-taps. Additionally, mapping out the logical routing—differentiating between what legally requires a nurse versus what can be directly fulfilled by an inventory technician—required deep thinking about hospital workflows and supply chain mechanics.

### Accomplishments that we're proud of

We are incredibly proud of the "Smart Routing" protocol. It is deeply satisfying to watch a patient press a button on a tablet and instantly see a mock Central Supply dashboard update, visually decrementing the stock of a medical device in real-time. We also successfully integrated text-to-speech functionality, ensuring the app announces the user's selection out loud, which provides immediate reassurance to the patient that their voice was heard.

### What we learned

We learned that supply chain optimization isn't just about shipping crates on cargo ships; it's about the localized, micro-logistics inside a building. If a hospital doesn't know where its specialized wheelchairs are, the supply chain is broken. We also learned how to implement strict ARIA labels and accessibility standards, realizing that good design for disabled users ultimately creates a cleaner, more efficient user experience for everyone.

### What's next for CareBridge

The next step is integrating a predictive AI forecasting model. As CareBridge collects data on which departments request specific durable medical equipment (DME) during specific times of the year, we can provide medical distributors with predictive analytics. Instead of hospitals placing reactive emergency orders for consumable supplies, CareBridge will eventually forecast demand, allowing suppliers to pre-stock inventory before a shortage ever occurs.

---

<a id="project-coderidge_adhd"></a>
## 26. CodeRidge_ADHD

- **Devpost:** [CodeRidge_ADHD](https://devpost.com/software/coderidge_adhd)
- **Crawl ID:** `coderidge_adhd`
- **Submitted to:** HackGwinnett 6.0
- **Built with:** css, github, javascript, json, react, websites

### Team

- [Tomii0415 Arowosegbe](https://devpost.com/Tomii0415)
- [Brandon Poole](https://devpost.com/bunny2027)
- [Luke](https://devpost.com/3am-la)
- [Sideswipe5](https://devpost.com/Sideswipe5)

### Project links

- [github.com/bunny2027/Hack_Gwinnett6.0-CodeRidge-](https://github.com/bunny2027/Hack_Gwinnett6.0-CodeRidge-)

### Images

- [Image 1](https://d112y698adiu2z.cloudfront.net/photos/production/software_photos/005/765/220/datas/original.jpg)
- [Image 2](https://d112y698adiu2z.cloudfront.net/photos/production/software_photos/005/765/221/datas/original.jpg)
- [Image 3](https://d112y698adiu2z.cloudfront.net/photos/production/software_photos/005/765/222/datas/original.jpg)
- [Image 4](https://d112y698adiu2z.cloudfront.net/photos/production/software_photos/005/765/223/datas/original.jpg)
- [Image 5](https://d112y698adiu2z.cloudfront.net/photos/production/software_photos/005/765/224/datas/original.jpg)
- [Image 6](https://d112y698adiu2z.cloudfront.net/photos/production/software_photos/005/765/225/datas/original.jpg)

### Technology references

- [css](https://devpost.com/software/built-with/css)
- [github](https://devpost.com/software/built-with/github)
- [javascript](https://devpost.com/software/built-with/javascript)
- [json](https://devpost.com/software/built-with/json)
- [react](https://devpost.com/software/built-with/react)

### Project description

- medical emergency form

- journal

- about section

- about section

- journal widgets

- home page

### Inspiration

Being a team of people who have background of being around those with Autism and ADHD, we wanted to build a website that would benefit them and their day to day life

### What it does

What it does it creates a platform where you can journal and talk about your day and make reminders about stuff you need to do and what you did in the following days in refence if you are interested in wat you did prior or any ideas that might have been overshot when being overtimulated

### How we built it

We built out website using a React Template and github to reference CSS designs, function, and formats, along with some help from stack overflow for debugging

### Challenges we ran into

- some challenges we faces were getting the form completely setup, Getting the css assets to blend together and stop overlapping, getting the form history to stop saving as a txt file instead of displaying, and trying to get the Medical location and for submission site together because the application rom the journal didn't transfer well to the medical form.

### Accomplishments that we're proud of

IT works, we are proud of that we were able to trouble shoot most of out problem, found repos that had the exact design we want to copy along with the functions too

### What we learned

- we learned that not all copy and pasted code can just fit in in work , we had to make our own personal changes to the website that would allow us to fit in all the styles we wanted

### What's next for CodeRidge_ADHD

Maybe the next step is learning how to integrate a map of the nearest medical center or maybe creating a small zen section to help with overstimulation.

---

<a id="project-visit-bridge"></a>
## 27. VisitBridge

- **Devpost:** [VisitBridge](https://devpost.com/software/visit-bridge)
- **Crawl ID:** `visit-bridge`
- **Submitted to:** HackGwinnett 6.0
- **Built with:** claude, react-native, typescript

### Team

- [ethan bui](https://devpost.com/ethanbuiquang)
- [Danny Lee](https://devpost.com/daenii066)

### Project links

- [github.com/dn0303/visitbridge](https://github.com/dn0303/visitbridge)

### Images

- [Image 1](https://d112y698adiu2z.cloudfront.net/photos/production/software_photos/005/765/102/datas/original.png)
- [Image 2](https://d112y698adiu2z.cloudfront.net/photos/production/software_photos/005/765/103/datas/original.png)
- [Image 3](https://d112y698adiu2z.cloudfront.net/photos/production/software_photos/005/765/104/datas/original.png)
- [Image 4](https://d112y698adiu2z.cloudfront.net/photos/production/software_photos/005/765/105/datas/original.png)

### Technology references

- [react-native](https://devpost.com/software/built-with/react-native)
- [typescript](https://devpost.com/software/built-with/typescript)

### Project description

- ai assistant

- settings

- id card

- scan

### Inspiration

We took inspiration from our own doctors visits and thinking about how difficult it might be for disabled people to check in. We designed VisitBridge to be very user-friendly and speed up the checking in process. We also remember being confused by doctor prescriptions or diagnoses, so we made VisitBridge simplify diagnoses and remind users to take medication.

### What it does

VisitBridge helps users check in more easily and understand doctors’ diagnoses. By giving them a daily check in, users do not have to remember when symptoms started, and information can be sent directly to doctors. Scanning prescriptions and diagnoses gives users more clarity about when to take medication or what next steps could be.

### How we built it

We first started by ideating, thinking about where we struggle when going to the doctors and how it might affect others with disabilities. Once landing on the check in process, we drew out the different pages and connected them with arrows to show how the buttons and other elements interact. We transferred this to Figma, a UI designing tool, and asked Claude to create our app. After a little bit of tweaking and small iterations, our final app was done.

### Challenges we ran into

We had some challenges with the app being “too AI” and implementing the AI agent to help users understand their diagnoses. We spent a lot of time redesigning and getting the api key for the AI assistant.

### Accomplishments that we're proud of

We are proud of our design process and how we used AI in a productive way while not being overly dependent. We’re also proud that we created an app that could help people walk through the medical care system, especially those with disabilities.

### What we learned

We learned how we could use AI to make our ideas real. We did not need to know how to code an entire website, only how to come up with an idea and design it.   We learned how to prompt AI effectively and efficiently.

### What's next for VisitBridge

For next steps, we want VisitBridge to be implemented in hospitals and clinics so that information can be sent directly to doctor’s offices.

---

<a id="project-ringroom"></a>
## 28. CareBridge Medical Assistant

- **Devpost:** [CareBridge Medical Assistant](https://devpost.com/software/ringroom)
- **Crawl ID:** `ringroom`
- **Submitted to:** HackGwinnett 6.0
- **Built with:** ai, css, googlescholar, html, javascript

### Team

- [Akbar Abbas Mirza](https://devpost.com/akbarabbasmirza)
- [Aidan Tao](https://devpost.com/aidant3304)

### Project links

- [relaxed-swan-0dd9ff.netlify.app](https://relaxed-swan-0dd9ff.netlify.app/)
- [sites.google.com/view/carebridge-health-assistant/full-page-embed](https://sites.google.com/view/carebridge-health-assistant/full-page-embed)

### Technology references

- [css](https://devpost.com/software/built-with/css)
- [html](https://devpost.com/software/built-with/html)
- [javascript](https://devpost.com/software/built-with/javascript)

### Project description

### Inspiration

The idea for CareBridge occured to us after discussing Akbar’s cousin in India. He lives with a cognitive disability where his mental processing develops at a different pace than his physical body, and because of his disability he had a distressing experience during a routine hospital checkup. Overwhelmed by the clinical environment, he was unable to communicate a simple point of distress—that his feet were freezing. The breakdown that followed was completely preventable, but highlighted a massive gap in healthcare: traditional hospital settings rely almost entirely on verbal, fast-paced patient communication.

After realizing and seeing how much strain frequent hospital visits put on both him and his parents, we realized that current hospital bedside tools aren't built for neurodivergent, non-verbal, or high-anxiety patients. We set out to build a tool that bridges the gap between patient bedsides and nursing stations, ensuring no patient's comfort or pain goes unheard.

### What it does

The app is intended to be an app easily accessible right from the hospital bed. The interface is easy to read, and features include:

- Quick help request buttons for general problems when the nurse is not in the room, such as pain, restroom assistance, and room accommodations.

- When workers are in the room and the patient is unable to speak, there is a wide variety of buttons using text-to-speech, ensuring the patient still has their requests met.

- Breakdown of medical terms such as "stat", "benign", etc.

- A page for the user to enter custom preferences as well as information of the hospital, patient name, room location, and care team.

### How we built it

We used prompt engineering, a handmade backbone of code and skills we learned for building websites in school courses to create a working website using HTML, CSS, and JavaScript that met all of our requirements that we wanted patients with disabilties in hospitals to be able to efficiently communicate with hospital staff.

### Challenges we ran into

Some challenges we faced while developing this app is focusing on the broader range of people with disabilities. Disabilities come in shapes and forms, which is why we brainstormed some common medical disabilities, and improved our web-app based on how we can effectviley support those disabilities in hospital. Besides the overall audience we are targeting our web-app, some technical problems within the design of the web-app also occured such as integrating the Web Speech API as it did not work the first couple times, although with some clever prompt engineering, and second hand sources we were able to effectively establish a Web Speech API into our website that works with pre-existing phrases and a separate option to input your own phrase.

### Accomplishments that we're proud of

The team built a proper tool that directly solves the exact problem that the team member's cousin faced, reducing lengthy requests down to a simple tap.

The application is also modeled after real world clinical software, making it easy to navigate and familiar.

### What we learned

We learned how to properly and effectively prompt engineer as our first few prompts were not going as intended, but after careful thinking we were able to design a prompt that gave us a very close to desired final product. Besides prompt engineering skills we were also able to learn some medical disabilities, and how to properly pertain our product to appeal to a wide range of patients with disabilities.

### What's next for CareBridge Medical Assistant

Right Now, we have a prototype that has our main core features fully functional, although actually establishing a system like this in hospitals needs a seperate end of the web-app so hospital staff can monitor and actually be able to communicate and provide the support patients need. The next steps for CareBridge is to establish a web-app for both ends of a hospital so that patient satisfaction and care for disabled patients is efficiently conducted from the patients to the hospital staff. After creating a fully working web-app for both ends of the hospital, we will pitch our idea to hospitals, and in the end create a succesful web-app that fosters efficient care for disbled patients and hospital staff.

### Password is My-Drop-Site for netlify

*No details provided in the crawl.*

---

<a id="project-beside-tqjhzm"></a>
## 29. Beside

- **Devpost:** [Beside](https://devpost.com/software/beside-tqjhzm)
- **Crawl ID:** `beside-tqjhzm`
- **Submitted to:** HackGwinnett 6.0
- **Built with:** claude, groq, html, javascript, python

### Team

- [Daniel](https://devpost.com/danitythemanity)
- [KickstarterX Laboy](https://devpost.com/KickstarterX)

### Project links

- [github.com/danitythemanity-cmd/beside.git](https://github.com/danitythemanity-cmd/beside.git)
- [besidehealth.vercel.app](http://besidehealth.vercel.app/)

### Images

- [Image 1](https://d112y698adiu2z.cloudfront.net/photos/production/software_photos/005/764/896/datas/original.png)
- [Image 2](https://d112y698adiu2z.cloudfront.net/photos/production/software_photos/005/764/897/datas/original.png)
- [Image 3](https://d112y698adiu2z.cloudfront.net/photos/production/software_photos/005/764/899/datas/original.png)
- [Image 4](https://d112y698adiu2z.cloudfront.net/photos/production/software_photos/005/764/900/datas/original.png)
- [Image 5](https://d112y698adiu2z.cloudfront.net/photos/production/software_photos/005/764/901/datas/original.png)
- [Image 6](https://d112y698adiu2z.cloudfront.net/photos/production/software_photos/005/764/927/datas/original.png)
- [Image 7](https://d112y698adiu2z.cloudfront.net/photos/production/software_photos/005/764/928/datas/original.png)
- [Image 8](https://d112y698adiu2z.cloudfront.net/photos/production/software_photos/005/764/929/datas/original.png)
- [Image 9](https://d112y698adiu2z.cloudfront.net/photos/production/software_photos/005/764/930/datas/original.png)
- [Image 10](https://d112y698adiu2z.cloudfront.net/photos/production/software_photos/005/764/931/datas/original.png)

### Technology references

- [groq](https://devpost.com/software/built-with/groq)
- [html](https://devpost.com/software/built-with/html)
- [javascript](https://devpost.com/software/built-with/javascript)
- [python](https://devpost.com/software/built-with/python)

### Project description

- Home Screen

- More of the Homepage

- Clinician Page

- Live Demo

- Patient Screen

- Pain describer, AI makes an overview and sends to doctor.

- Buttons for patient to communicate with doctor.

- AI simplifying medical wording

- Patient card so doctor knows how to interact with patient.

- Video call with patient.

### Inspiration

We wanted people who can't speak up for themselves to have a voice.

### What it does

It lets people who have a hard time speaking connect with doctors and feel included.

### How we built it

Mateo and I used a plethora of AI tools to build this.

### Challenges we ran into

GitHub was hard to work with, and we learned a lot of things from it.

### Accomplishments that we're proud of

We were able to integrate AI into it so it can easily translate different languages and make hard words simpler.

### What we learned

APIs are very helpful, and there is a huge community that does this kind of stuff.

### What's next for Beside

The sky is the limit.

---

<a id="project-carecost-7j0q23"></a>
## 30. CareCost

- **Devpost:** [CareCost](https://devpost.com/software/carecost-7j0q23)
- **Crawl ID:** `carecost-7j0q23`
- **Submitted to:** HackGwinnett 6.0
- **Built with:** ai, css, healthcare, healthcareaccessibility, healthcareeconomics, healthtech, html, javascript, react, tailwindcss, typescript, vite

### Team

- [jacobbweng Weng](https://devpost.com/jacobbweng)

### Project links

- [jacobbweng.github.io/CareCost](https://jacobbweng.github.io/CareCost/#map)

### Images

- [Image 1](https://d112y698adiu2z.cloudfront.net/photos/production/software_photos/005/764/911/datas/original.png)
- [Image 2](https://d112y698adiu2z.cloudfront.net/photos/production/software_photos/005/764/912/datas/original.png)
- [Image 3](https://d112y698adiu2z.cloudfront.net/photos/production/software_photos/005/764/913/datas/original.png)
- [Image 4](https://d112y698adiu2z.cloudfront.net/photos/production/software_photos/005/764/914/datas/original.png)
- [Image 5](https://d112y698adiu2z.cloudfront.net/photos/production/software_photos/005/764/915/datas/original.png)
- [Image 6](https://d112y698adiu2z.cloudfront.net/photos/production/software_photos/005/764/916/datas/original.png)
- [Image 7](https://d112y698adiu2z.cloudfront.net/photos/production/software_photos/005/764/917/datas/original.png)
- [Image 8](https://d112y698adiu2z.cloudfront.net/photos/production/software_photos/005/764/918/datas/original.png)

### Technology references

- [css](https://devpost.com/software/built-with/css)
- [html](https://devpost.com/software/built-with/html)
- [javascript](https://devpost.com/software/built-with/javascript)
- [react](https://devpost.com/software/built-with/react)
- [typescript](https://devpost.com/software/built-with/typescript)

### Project description

- Map, list of clinics

- Matches to your needs

- Insurance (Yes/No)

- Costs of a clinic

- Planning a Visit

- Overview of Clinics

- Map of Clinics

- Opening screen

As I started exploring healthcare accessibility, I became interested in the challenges people with disabilities encounter when trying to find a provider who can accommodate their needs.

Finding a doctor involves comparing prices, insurance, location, and availability. But for someone with a disability, there's even more to consider. Is the building wheelchair-accessible? Does the exam room have the necessary equipment? Are communication accommodations available? These questions can limit someone's options and sometimes force them to travel farther or spend more money to receive care.

That got me thinking about the financial side of accessibility. We usually measure healthcare costs by looking at the medical bill, but that's only part of the expense. Transportation, parking, and additional assistance can all contribute to the cost of receiving care. A provider with a lower appointment price isn't necessarily the most affordable option.

Thats why we made... CareCost.

I wanted to create a platform that considers accessibility and affordability together. Users can enter their individual accessibility requirements, identify which accommodations are essential, and find providers that best match their needs. Rather than simply recommending the cheapest option, CareCost considers whether a provider can actually accommodate the patient.

One of the main features I developed was the True Cost Calculator. It goes beyond the medical bill to estimate the additional expenses associated with accessing care. I also incorporated clinic costs, insurance analysis, and geographic accessibility into this personalized decision making process.

I built CareCost using React, TypeScript, Vite, and Tailwind CSS. One of the biggest challenges was bringing all these features together while making sure the recommendations were meaningful. Accessibility information isn't always complete. For example, a provider might have a wheelchair-accessible entrance but not an accessible examination room. I wanted CareCost to recognize when information was missing rather than automatically assuming a provider met someone's requirements.

Through this project, I learned how closely healthcare accessibility and economics are connected. A barrier that might seem small on paper can have a real financial impact on someone's ability to receive care. I also learned that building a useful recommendation system requires more than producing an answer. It means understanding the user's needs, accounting for different constraints, and being transparent about what the system does and doesn't know.

I'm proud of what I've built with CareCost, and I hope it helps people approach healthcare decisions with more information and fewer barriers.

Ultimately, I believe people shouldn't have to choose between healthcare that accommodates their needs and healthcare they can afford. CareCost is my attempt to help make both possible!

---

<a id="project-accessahead"></a>
## 31. AccessAhead

- **Devpost:** [AccessAhead](https://devpost.com/software/accessahead)
- **Crawl ID:** `accessahead`
- **Submitted to:** HackGwinnett 6.0
- **Built with:** css, figma, python, svg

### Team

- [souk xaya](https://devpost.com/souksom10)

### Project links

- [d3nrcrofvf4fa1.cloudfront.net/app](https://d3nrcrofvf4fa1.cloudfront.net/app/)

### Images

- [Image 1](https://d112y698adiu2z.cloudfront.net/photos/production/software_photos/005/764/926/datas/original.png)

### Technology references

- [css](https://devpost.com/software/built-with/css)
- [python](https://devpost.com/software/built-with/python)

### Project description

- These are the base design, then we used claude to input all of the functions we wanted in the app with this design.

### Inspiration

For many disabled people, the hardest part of healthcare starts before they ever step inside a clinic. A listing may claim a building is "wheelchair accessible," but that statement often applies only to the front door, leaving patients in the dark regarding exam tables, restrooms, interpreters, or waiting room sensory environments. The only way to discover these critical details is to phone the clinic—a process that presents a major barrier for Deaf patients, people with speech disabilities, neurodivergent individuals, and anyone managing severe fatigue. Arriving at a facility that cannot accommodate your needs wastes a trip that may have taken hours to arrange, often causing people to abandon seeking medical care entirely. We created AccessAhead to eliminate this hidden "pre-care" barrier so patients can know before they go.

### What It Does

AccessAhead is a mobile application that acts as an advocate for disabled patients. Users set their lasting accessibility needs once—covering mobility, hearing, vision, sensory, cognitive, and chronic illness considerations—and complete a quick daily check-in that re-ranks clinic results based on how they feel on any given day. Clinics are grouped into travel zones that display total matches alongside verified locations. Every clinic receives an Access Match Score that clearly explains itself, marking each detail as verified or unknown alongside its source and recency. For missing information, the app offers an "Ask for Me" feature that contacts the clinic directly to convert unknown details into verified facts. Additionally, the app includes a bill explainer that translates photographed medical statements into plain language to flag potential errors, as well as a visit preparation tool that generates one-tap accommodation requests and step-free directions.

### How We Built It

We developed AccessAhead using a mobile-first design strategy centered on strict digital accessibility. Starting with a palette of deep forest green, warm paper tones, and vermilion accents, we vetted every color pairing against WCAG 2.2 AA contrast standards, darkening borders and removing low-contrast states. Body text uses Atkinson Hyperlegible Next to assist readers with low vision, paired with Source Serif 4 for clear headings. Information status is always conveyed through combined text and icons rather than color alone, such as our "verified stamp" match score seal. We scripted our core assets and design system in Python as SVGs, imported them into Figma as editable frames, and maintained developer handoff using standardized CSS design tokens. The interface prioritizes physical ease of use through bottom-tab navigation, sticky primary buttons placed within thumb reach, tap targets exceeding 48 pixels, and an accessible text-resize option on every screen.

### Challenges We Ran Into

Building the platform presented several structural and technical hurdles. First, comprehensive clinic accessibility data simply does not exist in a single repository, forcing us to design a multi-source aggregation model that transparently displays data origins and highlights unknown fields rather than making assumptions. Second, balancing our high-concept visual inspiration with strict WCAG AA contrast guidelines required adjusting our palette, font weights, and element states. Mid-project, we also made the strategic decision to pivot from a desktop-focused web layout to a mobile-first phone app, which required rebuilding every screen into single-column layouts fitted for 390px viewports. Finally, accounting for fluctuating health conditions pushed us to expand beyond static user profiles, leading to the creation of our daily health check-in feature.

### Accomplishments That We're Proud Of

We are particularly proud of crafting a functional, fully WCAG 2.2 AA-compliant design system that maintains a warm, elegant visual identity without sacrificing contrast or legibility. We successfully built an honest, transparent scoring model that presents verified facts alongside unknown parameters, giving users clear expectations rather than false assurances. Our team seamlessly executed a complete mid-hackathon transition to a mobile-first architecture, redesigning our entire layout while preserving smooth developer handoff through structured CSS tokens. Most importantly, we engineered a platform that directly addresses the real-world barriers faced by disabled patients, transforming complex, scattered accessibility data into a dignified, user-centered care tool.

### What We Learned

This project reinforced that accessibility must be foundational rather than an afterthought, as contrast ratios, target sizes, screen-reader compatibility, and plain language dictated our interface decisions from day one. We also learned that structural honesty builds user trust; showing data sources and acknowledging missing information creates a far more reliable tool than making unverified claims. From a workflow perspective, establishing a clean handoff system with shared design tokens allowed our team to align design and development efforts smoothly under tight time constraints.

### What's Next for AccessAhead

Moving forward, we plan to expand AccessAhead by implementing post-visit community reviews to continuously crowdsource and refine clinic accessibility data. We aim to integrate accessible transportation booking features and provide downloadable, sign-language-translated versions of our visit preparation cards. Lastly, we intend to build a dedicated business portal where healthcare providers can directly claim their listings, update their accommodations, and verify their facility details.

---

<a id="project-benefitsbridge-d5bzl2"></a>
## 32. BenefitsBridge

- **Devpost:** [BenefitsBridge](https://devpost.com/software/benefitsbridge-d5bzl2)
- **Crawl ID:** `benefitsbridge-d5bzl2`
- **Submitted to:** HackGwinnett 6.0
- **Built with:** javascript, react, tailwind, typescript, vercel, vite

### Team

- [Anish Lanka](https://devpost.com/anish-l1202)
- [Abhiram Reddy](https://devpost.com/itsabhiramreddy)
- [Jamalsugger](https://devpost.com/Jamalsugger)

### Project links

- [benefitsbridge-chi.vercel.app](https://benefitsbridge-chi.vercel.app/)
- [github.com/anish1202-gif/BenefitsBridge](https://github.com/anish1202-gif/BenefitsBridge)

### Images

- [Image 1](https://d112y698adiu2z.cloudfront.net/photos/production/software_photos/005/765/081/datas/original.png)
- [Image 2](https://d112y698adiu2z.cloudfront.net/photos/production/software_photos/005/765/089/datas/original.png)
- [Image 3](https://d112y698adiu2z.cloudfront.net/photos/production/software_photos/005/765/090/datas/original.png)
- [Image 4](https://d112y698adiu2z.cloudfront.net/photos/production/software_photos/005/765/091/datas/original.png)
- [Image 5](https://d112y698adiu2z.cloudfront.net/photos/production/software_photos/005/765/092/datas/original.png)
- [Image 6](https://d112y698adiu2z.cloudfront.net/photos/production/software_photos/005/765/093/datas/original.png)
- [Image 7](https://d112y698adiu2z.cloudfront.net/photos/production/software_photos/005/765/094/datas/original.png)
- [Image 8](https://d112y698adiu2z.cloudfront.net/photos/production/software_photos/005/765/095/datas/original.png)
- [Image 9](https://d112y698adiu2z.cloudfront.net/photos/production/software_photos/005/765/096/datas/original.png)
- [Image 10](https://d112y698adiu2z.cloudfront.net/photos/production/software_photos/005/765/113/datas/original.png)
- [Image 11](https://d112y698adiu2z.cloudfront.net/photos/production/software_photos/005/765/114/datas/original.png)
- [Image 12](https://d112y698adiu2z.cloudfront.net/photos/production/software_photos/005/765/115/datas/original.png)
- [Image 13](https://d112y698adiu2z.cloudfront.net/photos/production/software_photos/005/765/116/datas/original.png)

### Technology references

- [javascript](https://devpost.com/software/built-with/javascript)
- [react](https://devpost.com/software/built-with/react)
- [typescript](https://devpost.com/software/built-with/typescript)

### Project description

About BenefitsBridge

Getting medical care with a disability can involve way more than visiting a doctor. You might need Medicaid, transportation, equipment, or financial assistance, but finding out what's available means searching through a bunch of different websites.

That's why I built BenefitsBridge.

It helps users find potential benefits, track applications, and figure out their next steps. There's also a Life Simulator that shows what might change if someone gets a job, moves, or has a change in income.

I built it using React, TypeScript, and Tailwind CSS. One challenge was making the recommendations useful without falsely promising eligibility.

BenefitsBridge also helps with the medical supply chain by guiding users through funding and paperwork for equipment like wheelchairs.

The goal is simple: make getting support less confusing.

---

<a id="project-pawthfinder-qagtbu"></a>
## 33. Pawthfinder

- **Devpost:** [Pawthfinder](https://devpost.com/software/pawthfinder-qagtbu)
- **Crawl ID:** `pawthfinder-qagtbu`
- **Submitted to:** HackGwinnett 6.0
- **Built with:** claude, css, gemini, html, javascript, python

### Team

- [awesomedudeguy6688 Conner](https://devpost.com/awesomedudeguy6688)

### Project links

- [github.com/awesomedudeguy6688/pawthfinder](https://github.com/awesomedudeguy6688/pawthfinder)

### Images

- [Image 1](https://d112y698adiu2z.cloudfront.net/photos/production/software_photos/005/765/186/datas/original.jpg)

### Technology references

- [css](https://devpost.com/software/built-with/css)
- [gemini](https://devpost.com/software/built-with/gemini)
- [html](https://devpost.com/software/built-with/html)
- [javascript](https://devpost.com/software/built-with/javascript)
- [python](https://devpost.com/software/built-with/python)

### Project description

- Concept of the Barnaby Pawthfinder Logo.

### Inspiration

Guide dogs help people with disabilities move through a world that wasn't built for them. They lead, warn about obstacles ahead, and let their handler make the decisions. We saw the same problem online, especially on patient portals, where people book appointments, refill medicines, and read test results. These sites are often full of tiny buttons, unlabeled forms, and hidden timers that sign you out and erase your work. So we built a guide dog for medical websites.

### What it does

Pawthfinder is a browser extension that sits on top of a patient portal and guides people through it, led by a friendly animated guide dog, Barnaby. Here are some main features that are of most importance to users:
Asks, doesn't assume - When you start, it asks what helps you: voice control, bigger text, plain words, keyboard use, and more. The site adapts instantly.
Leads the way - Say or type a goal like "Book a follow-up with my cardiologist." Barnaby turns it into a list of steps across several pages and walks you through each one.
Translates - It puts jargon into plain words, such as "Encounter Mgmt" becoming "Appointments", at three reading levels, and can read pages aloud.
“Sniffs” ahead - It warns you about barriers before you reach them, like mouse-only robot checks, fine-print payment agreements, and phone-only steps.
Protects your work - It spots hidden sign-out timers, keeps you signed in, and saves your answers.
Keeps you in control - It never fills in passwords and never ticks a consent box for you.
Stays private - Everything stays on your device, and it works offline.

### Challenges we ran into

We had no real patient portal we could test on, since real ones hold private health data. So we used Claude to build MyHealthLink, a mock portal with the barriers disabled patients really run into, built in on purpose: unlabeled fields, tiny mouse-only buttons, a mouse-only robot check, and a hidden four-minute sign-out. That gave us a realistic "before" to compare against Pawthfinder's "after".
We also had to design for many disabilities at once without forcing anyone into one category. That led us to replace fixed presets with a "what helps you?" picker.

### Accomplishments we're proud of

We built AI test agents that act as disabled users:  The agents found real problems a sighted mouse user would never notice, like keyboard focus getting lost after closing a notice. That gave us a prioritized list of fixes.

### What we learned

AI works best with focused jobs, not one giant prompt. We split the work across specialist agents: one for performance, one for visual design, one to test as disabled users, and a manager agent that checks everyone's work against our goals and stops agents from overwriting each other. We learned to give each agent clear rules about which files it owns. We also learned that accessibility has to win whenever it conflicts with looks or speed.

### What's next for Pawthfinder

More portals - Use an AI model to understand any medical website, not just our demo, while keeping health data on the device.
Connect to care - Link Pawthfinder to real portal systems so people can reach their doctors, send accommodation requests, and keep appointments in sync.
Test with real people - Run the app with disabled users, screen readers, and voice-control software, not just simulations.

---

<a id="project-access-care-navigator"></a>
## 34. Access Care Navigator

- **Devpost:** [Access Care Navigator](https://devpost.com/software/access-care-navigator)
- **Crawl ID:** `access-care-navigator`
- **Submitted to:** HackGwinnett 6.0
- **Built with:** css, typescript

### Team

- [Arjun Chakraborty](https://devpost.com/arjunch5045)
- [Anish Kidambi](https://devpost.com/anishkid09)
- [Praval](https://devpost.com/praval-gamex3)

### Project links

- [github.com/Vortezler/access-care-navigator](https://github.com/Vortezler/access-care-navigator)
- [access-care-navigator.vercel.app](https://access-care-navigator.vercel.app/)

### Technology references

- [css](https://devpost.com/software/built-with/css)
- [typescript](https://devpost.com/software/built-with/typescript)

### Project description

Access Care Navigator

### Inspiration

People with disabilities often face additional challenges when trying to access healthcare. Finding a medical provider is already difficult, but finding one that can accommodate specific disabilities, treat a patient's medical conditions, and accept their insurance can make the process even more complicated. Patients often have to spend hours researching different clinics, contacting providers, and figuring out which facilities can actually meet their needs.

We wanted to address this problem by creating a platform that simplifies the entire healthcare search process. Our goal was to use AI to make healthcare more accessible by helping people find providers who understand their individual circumstances and can properly support them.

### What It Does

Access Care Navigator is an AI-powered healthcare navigation platform designed to make finding appropriate medical care easier for people with disabilities.

Users can communicate with our AI chatbot through voice or text to explain their disabilities, symptoms, and existing medical conditions. They can also upload medical documents and PDFs to provide additional context about their medical history.

Using this information, the platform searches for nearby medical clinics and evaluates how well each facility can accommodate the user's specific disabilities. It also considers whether the clinic has qualified professionals who can address the user's symptoms or medical conditions and whether the facility accepts their insurance.

Rather than simply providing a list of nearby clinics, Access Care Navigator helps narrow down the options to providers that are actually suitable for each individual. The chatbot can also analyze the information provided, identify potential medical concerns, and offer general guidance and suggestions to help users manage their symptoms while seeking appropriate care.

Once a suitable clinic is identified, the platform confirms the recommendation with the user before proceeding. It can draft and send emails to clinics, assist with appointment scheduling, and even book appointments directly when supported by the provider. If direct booking is unavailable, it guides users to the appropriate website or contact information.

Our goal is to reduce the time, frustration, and uncertainty involved in finding accessible healthcare by allowing users to explain their needs once and letting AI handle much of the research and coordination for them.

### How We Built It

We began by identifying a real-world problem and developing an idea for how AI could help address it. After establishing the main features and requirements of our platform, we used Claude as a development assistant to help generate and refine the code.

However, building the platform involved much more than simply asking AI to write code. We spent considerable time planning the functionality, explaining our requirements, testing different features, identifying errors, and repeatedly revising the implementation to match our original vision.

We worked on bringing several interconnected features together, including the voice chatbot, medical document analysis, symptom analysis, disability-specific clinic matching, insurance compatibility, and appointment coordination. Making sure these features worked together properly required multiple rounds of testing and troubleshooting.

Throughout development, we continuously evaluated the results, adjusted our instructions, and worked through problems until the platform better reflected what we wanted to accomplish. It was a process of constant refinement, and each stage helped us improve the overall functionality and user experience.

### Challenges We Ran Into

One of our biggest challenges was getting AI to understand exactly what we wanted to build. Since our platform included several different features that needed to work together, giving general instructions often resulted in code that did not fully match our expectations.

We frequently had to go back, explain specific requirements in greater detail, identify what was missing, and request changes. Sometimes fixing one issue created another, which meant we had to repeatedly test different parts of the platform and troubleshoot problems.

Another challenge was making sure that our features worked together as one connected system rather than as separate functions. We had to spend a significant amount of time refining the code and adjusting the implementation to create a more complete experience.

Although the process was sometimes frustrating, it taught us the importance of patience, clear communication, and persistence when developing a complex project.

### Accomplishments That We're Proud Of

We are especially proud of turning an idea focused on a real-world accessibility problem into a functioning AI-powered platform. Instead of creating another basic medical chatbot or clinic finder, we wanted to build something that could assist users throughout the entire process of finding appropriate healthcare.

One of our biggest accomplishments was bringing together multiple features into one platform. Access Care Navigator considers a user's medical needs, disabilities, required accommodations, insurance coverage, and location when recommending healthcare providers.

We are also proud of developing a system that goes beyond simply recommending clinics. It can help users understand their potential medical concerns, find suitable professionals, communicate with clinics, and navigate the appointment scheduling process.

Most importantly, we are proud of the amount of effort we put into developing and refining our original idea. We encountered several technical challenges, but we continued testing, troubleshooting, and improving the platform instead of settling for an incomplete first version. Seeing our original concept develop into something that could potentially make a meaningful difference in people's lives has been one of our greatest accomplishments.

### What We Learned

One of the biggest things we learned throughout this project is that while AI is a powerful tool that can do a lot of the work, it still requires human guidance. We realized that simply giving AI a general idea of what we wanted was not enough to get the best results.

We had to be specific about our requirements, continuously provide instructions, and make adjustments whenever something did not work as intended. AI does not always recognize its own mistakes or know how to improve something in the way we envision, so it was our responsibility to identify problems, evaluate its results, and guide it toward a better solution.

This taught us that AI works best when combined with human creativity, critical thinking, and problem-solving rather than being relied on to do everything independently.

We also learned more about web development, debugging, integrating different technologies, and the importance of designing technology with accessibility in mind. Most importantly, we learned that technology can be used for more than convenience; it can help address real-world problems and make important services more accessible to people who need them.

### What's Next for Access Care Navigator?

We hope to continue expanding and improving Access Care Navigator by increasing the number of medical providers available in its database and improving the accuracy of its recommendations.

In the future, we would like to expand its ability to recognize different disabilities and match users with more specific accommodations. We also want to improve its medical document analysis, integrate with more insurance providers, and make appointment scheduling available through a wider range of clinics.

Another important goal is improving the chatbot's ability to maintain context throughout the user's experience, allowing people to explain their circumstances once without having to repeatedly provide the same information.

Ultimately, we envision Access Care Navigator becoming a reliable healthcare navigation tool that removes unnecessary barriers for people with disabilities. We want to make finding appropriate healthcare less stressful, more efficient, and more accessible so that people can focus less on searching for care and more on receiving it.

---

<a id="project-clinic-admitter"></a>
## 35. Clinic Admitter

- **Devpost:** [Clinic Admitter](https://devpost.com/software/clinic-admitter)
- **Crawl ID:** `clinic-admitter`
- **Submitted to:** HackGwinnett 6.0
- **Built with:** codehs, java

### Team

- [Gerald Nwaka](https://devpost.com/gndevcode)

### Project links

- [github.com/gndevcode/Clinic-Admitter__HackGwinnet6.0](https://github.com/gndevcode/Clinic-Admitter__HackGwinnet6.0)

### Images

- [Image 1](https://d112y698adiu2z.cloudfront.net/photos/production/software_photos/005/765/208/datas/original.png)

### Technology references

- [java](https://devpost.com/software/built-with/java)

### Project description

- Output of the program

### Inspiration

Creating an inclusive appointment system for clinics

### What it does

Orders and allots accommodations of patients for clinics

### How we built it

CodeHS

### Challenges we ran into

Ordering the patients by priority

### Accomplishments that we're proud of

The program works smoothly and as intended

### What we learned

Arrays and loops are needed to allot by priority

### What's next for Clinic Admitter

Inclusion of more accommodations; better UX

---

<a id="project-adaptive-touch"></a>
## 36. Adaptive Touch

- **Devpost:** [Adaptive Touch](https://devpost.com/software/adaptive-touch)
- **Crawl ID:** `adaptive-touch`
- **Submitted to:** HackGwinnett 6.0
- **Built with:** chatgpt, intellij-idea, python, swift

### Team

- [Roman K](https://devpost.com/roma-krutov11)
- [Ayaan Tuteja](https://devpost.com/ayaan-tuteja06)

### Project links

- [github.com/Roman110311/Hackathon-AI-Division](https://github.com/Roman110311/Hackathon-AI-Division)

### Images

- [Image 1](https://d112y698adiu2z.cloudfront.net/photos/production/software_photos/005/765/194/datas/original.png)
- [Image 2](https://d112y698adiu2z.cloudfront.net/photos/production/software_photos/005/765/195/datas/original.png)
- [Image 3](https://d112y698adiu2z.cloudfront.net/photos/production/software_photos/005/765/198/datas/original.png)
- [Image 4](https://d112y698adiu2z.cloudfront.net/photos/production/software_photos/005/765/197/datas/original.png)
- [Image 5](https://d112y698adiu2z.cloudfront.net/photos/production/software_photos/005/765/196/datas/original.png)

### Technology references

- [intellij-idea](https://devpost.com/software/built-with/intellij-idea)
- [python](https://devpost.com/software/built-with/python)
- [swift](https://devpost.com/software/built-with/swift)

### Project description

- Title slide

- Table of contents

- Research prompt

- Background

- Purpose

### Inspiration

My cousin was volunteering at a library and told me about the struggles that seniors experience due to the hand tremors. She suggested that we work together to create a hardware project which could help solve the issue. It ended up not working out, so we decided to implement it using software.

### What it does

AdaptiveTouch makes a healthcare navigation easier to use for people with hand tremors or difficulty making precise touches. It responds to phone movement, provides larger touch targets, tolerates small finger movements, and helps prevent accidental taps. Users can also adjust these features and schedule fictional appointments.

### How we built it

We built AdaptiveTouch as a native iPhone app using Swift, SwiftUI, UIKit, and Core Motion. It combines sensor-assisted interface movement with larger touch targets, touch tolerance, and accidental-tap protection in a fictional healthcare portal demo and theoretically applies to any software, especially healthcare related software.

### Challenges we ran into

Making motion compensation smooth and readable was difficult. Early versions reacted too strongly to phone tilt, so we focused on lateral acceleration and added smoothing. We also worked to make touch controls forgiving while preserving scrolling.

### Accomplishments that we're proud of

We created a working iPhone prototype that brings the accessibility features together. Users can adjust settings, compare touch modes, and book fictional appointments through a confirmation flow.

### What we learned

Accessibility features need to be adjustable. Each person has different gyroscopic movement for trembling and intentional movement.  We also learned that motion sensors can estimate short-term movement but can’t reliably track the phone’s exact position.

### What's next for Adaptive Touch

We want to test with more users, refine motion and touch handling, improve calibration, make it immediately applicable to any software with ease, and expand accessibility and VoiceOver testing.

NOTE FOR THE GITHUB LINK: In order to test this process, you must run it through Xcode on a Mac, and run it through a connected iPhone. The program is built specifically for updated iPhones and simulating the program through a Mac yields the intended result. Please do not try using this in any other scenarios, it will not work.
YOU MUST USE THE ROMAN DIRECTORY. DO NOT USE THE MAIN ONE. IT IS UNOPTIMIZED. THANK YOU FOR UNDERSTANDING. WE APPRECIATE YOU!

---

<a id="project-accessible-medical-care-navigator"></a>
## 37. Accessible Medical Care Navigator

- **Devpost:** [Accessible Medical Care Navigator](https://devpost.com/software/accessible-medical-care-navigator)
- **Crawl ID:** `accessible-medical-care-navigator`
- **Submitted to:** HackGwinnett 6.0
- **Built with:** react

### Team

- [Cloudy Sanjesh](https://devpost.com/ishaan-sanjesh)
- [loloheria Hung](https://devpost.com/loloheria)
- [Aarmaan Singh](https://devpost.com/aarmaansingh-prof)

### Project links

- [drive.google.com/file/d/1zABICu95d4EZOw4NpW8YGB2xQGPSZQnb/view](https://drive.google.com/file/d/1zABICu95d4EZOw4NpW8YGB2xQGPSZQnb/view?usp=sharing)

### Technology references

- [react](https://devpost.com/software/built-with/react)

### Project description

### Inspiration

We were inspired by Google FitBit's AI assistant giving personalized workout information and thought that this could be developed into a website that helps to simplify the navigation of medical care. This process is unique to each person, so we thought of using AI to personalize it, especially for specific disabilities.

### What it does

Takes photos of medical forms/documents (not including insurance, billing, etc.) and translates them into laypeople speak. This can be done through manual input or speaking input (speech to text assistance). When analyzing the documents, it catches and removes personal information like emails, phone numbers, and user IDs. The simplified version of the test will be displayed in a side-by-side format with the original. The user can click on certain sections of the simplified document and the corresponding translation will be highlighted in the original version. The user can also ask clarifying questions about the document by speaking or text input. Spoken questions will be answered aloud, while typed answers will have a “read aloud” option. Any answers that cannot be found in the document will return “Not in this document”.

### How we built it

TypeScript and React with accessible components
(React Aria). The same code runs as a website, an installable offline app, a
Windows/Linux desktop app (Tauri), and an Android app (Capacitor).

### Challenges we ran into

OCR found only about 43% of key phrases on phone-style photos at
first. We built an evaluation harness and tested cleanup steps one at a time.
Removing shadows helped dim photos a lot but hurt clean pages, so we made it
conditional. Picking results by OCR confidence backfired, so we dropped it.

### What's next for Accessible Medical Care Navigator

We would like to add support for different languages, as there are many who many not be proficient in English or are more comfortable reading in another language. Additionally, we would like to add walkthroughs, where an AI assistant can walk one through making an appointment or filling out a form. This would be helpful for those unfamiliar with the process or for those with cognitive impairment. It would provide things like checklists that will clarify the process/remind users.

Video Link:https://drive.google.com/file/d/1zABICu95d4EZOw4NpW8YGB2xQGPSZQnb/view?usp=sharing

---

<a id="project-healthbridge-sif8ny"></a>
## 38. HealthBridge

- **Devpost:** [HealthBridge](https://devpost.com/software/healthbridge-sif8ny)
- **Crawl ID:** `healthbridge-sif8ny`
- **Submitted to:** HackGwinnett 6.0
- **Built with:** css, html, javascript

### Team

- [Amit Kamal Mudududla](https://devpost.com/amitkamalmudududla)
- [Levi Jones](https://devpost.com/r1chyj4492)

### Project links

- [github.com/Amit-Kamal/HealthBridge](https://github.com/Amit-Kamal/HealthBridge)

### Images

- [Image 1](https://d112y698adiu2z.cloudfront.net/photos/production/software_photos/005/765/419/datas/original.png)

### Technology references

- [css](https://devpost.com/software/built-with/css)
- [html](https://devpost.com/software/built-with/html)
- [javascript](https://devpost.com/software/built-with/javascript)

### Project description

- A picture of working application.

Over 25% of adults live with a disability, yet online healthcare portals routinely block them with unlabeled forms, poor contrast, and complex navigation. When digital tools fail, patients often blame themselves. We built HealthBridge to put the power back in patients' hands.
HealthBridge is a Manifest V3 browser extension and accessibility copilot designed by team Verities. It is not an overlay—it runs only when triggered by the user. It adapts their view in real time and provides an automated WCAG 2.1 compliance report card without compromising privacy or claiming false site-wide compliance.

### How we built it

Core Extension: Built using Vanilla JavaScript, ES modules, and Manifest V3.
Scanner: Powered by axe-core to run WCAG 2.1 A/AA compliance checks directly on active tabs.
Side Panel UI: A custom, accessible 4-tab interface for scanning pages, simplifying text into a Reader View, navigating forms step-by-step, and applying instant display preferences (high contrast, text spacing, and strong focus rings) via chrome.storage.sync.
Form Helper & Write-Back: Safely maps form elements, bypassing brittle selectors to inject values using native setters and event dispatchers so modern framework forms recognize the changes.
AI Features: We also created specific AI features to further help users.

### Challenges we ran into

Handling dynamic DOM changes across various healthcare portal structures without breaking user input.
Ensuring strict adherence to our non-overlay philosophy by routing all interactions locally on-device and using optional host permissions.

### Accomplishments that we're proud of

Delivering a fully functional, end-to-end prototype featuring an automated WCAG auditor, a clean Reader View, and an interactive form wizard within the hackathon timeframe.

---

<a id="project-barry-b5adrc"></a>
## 39. Barry

- **Devpost:** [Barry](https://devpost.com/software/barry-b5adrc)
- **Crawl ID:** `barry-b5adrc`
- **Submitted to:** HackGwinnett 6.0
- **Built with:** amazon-web-services, aws-transcribe, claude, codex, css, git, html, next.js, npm, s3, typescript, vscode

### Team

- [Virgil Holmes](https://devpost.com/virgilholmes)
- [Justin Pongpairoj](https://devpost.com/justin-pongpairoj)
- [Austin Dixon](https://devpost.com/theblur4900)

### Project links

- [github.com/virgilholmes/barry](https://github.com/virgilholmes/barry)

### Technology references

- [amazon-web-services](https://devpost.com/software/built-with/amazon-web-services)
- [css](https://devpost.com/software/built-with/css)
- [git](https://devpost.com/software/built-with/git)
- [html](https://devpost.com/software/built-with/html)
- [npm](https://devpost.com/software/built-with/npm)
- [typescript](https://devpost.com/software/built-with/typescript)

### Project description

Barry’s web interface and application logic are built on Next.js, delivering a responsive, high-contrast black, white, and orange interface. We integrated Supabase for user authentication and relational/vector storage, creating a secure, persistent memory vault that locks in a user's medical history, accommodations, and communication preferences after a single briefing. To power live appointment mode, we integrated Amazon Transcribe to handle high-accuracy, low-latency clinical speech-to-text. This allows Barry to listen to rapid doctor-patient conversations in real time, bridging the communication speed gap for non-verbal users and those with speech impairments. The core advocacy engine relies on Claude hosted via Amazon Bedrock, orchestrating complex contextual reasoning, real-time response generation, and post-visit insurance appeal automation. Development was accelerated using Codex and OpenCode for agent workflow automation, code generation, and rapid iteration during the hackathon.

Balancing low-latency streaming between Next.js, Amazon Transcribe, and Amazon Bedrock was a major hurdle. In live clinical settings, non-verbal patients need near-instantaneous advocacy generation without sacrificing Claude’s medical reasoning accuracy. Structuring Supabase memory persistence to carry over critical accommodation needs without cluttering the context window with irrelevancies from past appointments required careful prompt engineering and state management in Next.js. Designing a modern interface with a black, white, and orange palette while adhering strictly to high-contrast WCAG AAA accessibility standards meant carefully tuning accent colors and typography so screen readers and visually impaired users experience zero visual fatigue.

Designing for non-verbal and chronically ill users forced us to build cleaner Next.js component architectures, tighter API payloads, and far more intuitive user flows than a standard healthcare app would ever require. Moving away from single-session chat models to persistent agentic companions completely eliminates repetition fatigue. One briefing changes how patients experience healthcare forever. AI in healthcare should never act as a black-box replacement for doctors or patients; it must serve as an empowered, user-controlled advocate that amplifies the patient's own voice.

---

<a id="project-simplejargon"></a>
## 40. SimpleJargon

- **Devpost:** [SimpleJargon](https://devpost.com/software/simplejargon)
- **Crawl ID:** `simplejargon`
- **Submitted to:** HackGwinnett 6.0
- **Built with:** css3, ejs, express.js, html5, javascript, node.js

### Team

- [Jay Zhou](https://devpost.com/non-reai)

### Project links

- [github.com/non-reai/HackGwinnett2026](https://github.com/non-reai/HackGwinnett2026)

### Images

- [Image 1](https://d112y698adiu2z.cloudfront.net/photos/production/software_photos/005/765/078/datas/original.png)
- [Image 2](https://d112y698adiu2z.cloudfront.net/photos/production/software_photos/005/765/079/datas/original.png)
- [Image 3](https://d112y698adiu2z.cloudfront.net/photos/production/software_photos/005/765/080/datas/original.png)

### Technology references

- [css3](https://devpost.com/software/built-with/css3)
- [ejs](https://devpost.com/software/built-with/ejs)
- [express-js](https://devpost.com/software/built-with/express-js)
- [html5](https://devpost.com/software/built-with/html5)
- [javascript](https://devpost.com/software/built-with/javascript)
- [node-js](https://devpost.com/software/built-with/node-js)

### Project description

- Patient Dashboard

- Homepage

- Post-visit Data provided by doctor (mock data)

### Inspiration

I felt like one of the biggest disconnects in healthcare is the gap between the visit to the doctor's and post visit. Sometimes I don't remember all the details of what my doctor said. That was my inspiration to create this project.

### What it does

The idea is that this platform has both doctors and patients. After a patient leaves, the doctor uses the doctor portal on the website to instruct the patient on what to do after and what medications to take with what frequency.

### How we built it

I used WebStorm to build it which is a very nice IDE for web development. I coded this with EJS and NodeJS and HTML/CSS/JS stack.

### Challenges we ran into

I do not know the medical world that much. I struggled with finding solutions I could help with. Another challenge I encountered was a lot of empty space on the UI and I could not fill it up. UI design was a pain in general with this project.

### Accomplishments that we're proud of

I am proud that I was able to develop a small demo in 4 hours, especially with my lack of background knowledge in this area.

### What we learned

I learned a lot about how inefficient the healthcare system is, with how many forms patients have to fill out. My original direction was to make a document simplifier but even I could not figure out how the forms worked.

### What's next for SimpleJargon

I want to create an account system and overhaul the UI to make it much more visually appeasing and accessible.

---

<a id="project-memory-preservation-game"></a>
## 41. Memory Preservation Game

- **Devpost:** [Memory Preservation Game](https://devpost.com/software/memory-preservation-game)
- **Crawl ID:** `memory-preservation-game`
- **Submitted to:** HackGwinnett 6.0
- **Built with:** chatgpt, visual-studio

### Team

- [Leon Ehima](https://devpost.com/leonehima2022)

### Project links

- [github.com/Leonprogrammer2346/RESTARANTHACK2](https://github.com/Leonprogrammer2346/RESTARANTHACK2)

### Images

- [Image 1](https://d112y698adiu2z.cloudfront.net/photos/production/software_photos/005/765/229/datas/original.png)

### Technology references

- [visual-studio](https://devpost.com/software/built-with/visual-studio)

### Project description

### Inspiration

Memory Loss Patients

### What it does

Tests Memory

### How we built it

In My Personal Game Engine

### Challenges we ran into

The Deadline

### Accomplishments that we're proud of

no

### What we learned

didly squat

### What's next for Memory Preservation Game

the deleted folder

---

<a id="project-care-helper"></a>
## 42. Care Helper

- **Devpost:** [Care Helper](https://devpost.com/software/care-helper)
- **Crawl ID:** `care-helper`
- **Submitted to:** HackGwinnett 6.0
- **Built with:** github, python

### Team

- [Tim McCall](https://devpost.com/trmccall31)
- [Mobley](https://devpost.com/avontemobley9)

### Project links

- [github.com/LemonLD31/hackathonBlacks](https://github.com/LemonLD31/hackathonBlacks)

### Technology references

- [github](https://devpost.com/software/built-with/github)
- [python](https://devpost.com/software/built-with/python)

### Project description

### Inspiration

We wanted to help people with online medical issues.

### What it does

It asks for the issue and give a solution.

### How we built it

We used the inbuilt code software in GitHub and used the python language.

### Challenges we ran into

The biggest challenge was creating an Idea for the project.

### Accomplishments that we're proud of

The project was an accomplishment for us beginner coders.

### What we learned

We learned more about GitHubs software

### What's next for Care Helper

We plan to improve the code and use it for greater purposes later down the road.

---

<a id="project-avaneesh-nelakosigi"></a>
## 43. Avaneesh Nelakosigi

- **Devpost:** [Avaneesh Nelakosigi](https://devpost.com/software/avaneesh-nelakosigi)
- **Crawl ID:** `avaneesh-nelakosigi`
- **Submitted to:** HackGwinnett 6.0
- **Built with:** claude, css3, github, html5, javescript

### Team

- [prodradjr Nelakosigi](https://devpost.com/prodradjr)

### Project links

- [prodradjr.github.io/HospitalRating/HospitalRating](https://prodradjr.github.io/HospitalRating/HospitalRating/#needs)

### Technology references

- [css3](https://devpost.com/software/built-with/css3)
- [github](https://devpost.com/software/built-with/github)
- [html5](https://devpost.com/software/built-with/html5)

### Project description

### Inspiration

The theme was accessibility in navigating the medical system, so I started by looking at what actually stops disabled patients from getting care. One problem kept coming up: inaccessible medical equipment. Fixed-height exam tables, standard scales, no patient lifts. Wheelchair users are often examined sitting in their chair, or not weighed at all, which affects diagnosis and medication dosing.

Then I tried to find out which Atlanta hospitals have accessible equipment. I checked the official websites of Emory, Piedmont and Grady hospitals. None of them published it. Patients only find out when they arrive.

Reviews don't fill the gap either. A one-star review might be about parking while the lift worked perfectly, and a five-star review might come from someone who couldn't get onto the exam table. One star rating can't tell a wheelchair user whether the equipment they need works.

### What it does

HospitalRating shows, for every place and every piece of accessibility equipment, what the hospital says next to what patients say, and warns when the two don't match.

- Choose your needs: adjustable exam table, wheelchair scale, patient lift, accessible restroom, step-free entrance, staff help, accessible mammography.

- Browse 23 real places in metro Atlanta and Gwinnett: 8 hospitals, 7 urgent care centers and 8 specialist clinics (ENT, cardiology, orthopedics, breast imaging).

- See match scores like "Patients confirm 3 of 4 of your needs."

- Write a review in your own words, typed or spoken. The app reads it sentence by sentence and updates the results live. Stars are never used.

- Call the clinic or get directions in Google Maps or Apple Maps with one tap.

### How I built it

- Plain HTML, CSS and JavaScript. No frameworks, no server, no accounts, so it runs anywhere, even offline, and is hosted on GitHub Pages.

- Machine learning written from scratch: two Naive Bayes text classifiers in JavaScript. Each review is split into sentences. The first classifier decides which equipment the sentence is about (or "other," like parking, which is ignored). The second decides whether it worked or failed. If confidence is below 60%, the app asks the user to confirm instead of guessing, and users can correct mistakes with one tap.

- Training data: 162 labelled sentences written in the casual, run-on, sometimes misspelled way people actually write reviews.

- Evaluation: a Node.js script holds out 20% for testing. Item accuracy is 93.8%, and 96.6% when the model is confident. Worked/failed accuracy is 81.3%.

- Voice input uses the Web Speech API, with clear error messages and a typing fallback.

- Real data: hospital names, addresses and phone numbers were checked against official websites. Places I couldn't check are tagged "unverified."

- I used Claude Code, an AI coding assistant, to help plan and write the code.

### Challenges I ran into

- The data doesn't exist. I couldn't find any public source for hospital accessibility equipment. That became the core of the project instead of a blocker: every hospital honestly shows "Not published," and patients fill the gap.

- Staying honest with real hospitals. Made-up negative reviews about real hospitals would be false claims. All demo reviews are clearly labelled, and I never invented an equipment claim.

- Verifying data: some hospital websites blocked my checks, so those places are marked unverified instead of guessed.

- Voice input only works in some browsers and only over a secure connection, which took debugging.

- Worked vs. failed is harder than it looks. Sentences like "the table was supposed to lower but nobody knew how" mix both, which is why that classifier is less accurate than the item classifier.

- Changing direction: I explored several other ideas before landing on this one, with limited time and working solo.

### Accomplishments I'm proud of

- Machine learning I built and can fully explain, with real accuracy numbers, including where it gets confused.

- Turning a 1-star review into useful equipment information ("lift: worked") instead of a penalty.

- An app that is accessible itself: large text with size controls, keyboard navigation, screen reader support, and icons plus words instead of color alone.

- Using real hospitals while staying honest about what's demo data.

### What I learned

- Accessibility problems are often information problems: the equipment might exist, but nobody tells the patient.

- A single rating hides the details that matter most to disabled users.

- A small, well-chosen ML model you can measure is more useful, and easier to trust, than a big one you can't explain.

### What's next

- Hospitals publishing their own equipment data. The 2024 federal rule on accessible medical equipment gives them a reason to.

- Confirming reviews come from a real visit, to stop fake reviews.

- More training data from real patients, more languages, and coverage across Georgia.

---

<a id="project-visitvoice"></a>
## 44. VisitVoice

- **Devpost:** [VisitVoice](https://devpost.com/software/visitvoice)
- **Crawl ID:** `visitvoice`
- **Submitted to:** HackGwinnett 6.0
- **Built with:** codehs, html

### Team

- [Vivek Sing](https://devpost.com/vivekzing20)
- [Jonathan03312011 Jan](https://devpost.com/Jonathan03312011)
- [William Im](https://devpost.com/williamim089)

### Project links

- [drive.google.com/file/d/1dicwRekjJ84hA3EQ58vZYentRk2myUhu/view](https://drive.google.com/file/d/1dicwRekjJ84hA3EQ58vZYentRk2myUhu/view?ts=6ae63a3d)
- [new-sandbox-program-19-21591485.codehs.me/index.html](https://new-sandbox-program-19-21591485.codehs.me/index.html)

### Images

- [Image 1](https://d112y698adiu2z.cloudfront.net/photos/production/software_photos/005/765/236/datas/original.jpg)

### Technology references

- [html](https://devpost.com/software/built-with/html)

### Project description

To start, many autistic children or people with learning disabilities have a problem with expressing themselves the proper way. Thus, we decided to create a project that helps children/adults with disabilities to express themselves the right way, by pressing buttons that produce audio to express the person's opinions. We built our project using HTML and CSS. Since we do not have a lot of experience with generating UI and input platforms, we found it challenging for the design and overall aesthetics of the platform.

Go to this: https://drive.google.com/file/d/1dicwRekjJ84hA3EQ58vZYentRk2myUhu/view?ts=6ae63a3d

---

<a id="project-accessmed"></a>
## 45. AccessMed

- **Devpost:** [AccessMed](https://devpost.com/software/accessmed)
- **Crawl ID:** `accessmed`
- **Submitted to:** HackGwinnett 6.0
- **Built with:** css, html, javascript, json

### Team

- [Raydan Valrie](https://devpost.com/raydanvalrie09)

### Project links

- [github.com/RaydanV/Workshop/tree/main/accessmed](https://github.com/RaydanV/Workshop/tree/main/accessmed)

### Technology references

- [css](https://devpost.com/software/built-with/css)
- [html](https://devpost.com/software/built-with/html)
- [javascript](https://devpost.com/software/built-with/javascript)
- [json](https://devpost.com/software/built-with/json)

### Project description

### Inspiration/Context

Healthcare management has rapidly shifted online, but patient portals are notoriously difficult to navigate. For millions of individuals—including seniors, people with visual or motor disabilities, and those with low health literacy—booking an appointment, checking lab results, or understanding a medical bill can feel like an impossible task. Missing an appointment or misunderstanding dosage instructions isn't just a minor inconvenience; it’s a real health risk.

We were inspired to build AccessMed to ensure that digital healthcare is an accessible right for everyone, regardless of physical capability or medical knowledge.

### What it does

AccessMed is a client-side browser extension (Manifest V3) that acts as an intelligent accessibility and plain-language layer over any patient portal (such as Epic, MyChart, or Athenahealth).

Visual Enhancements: Auto-detects and injects missing aria-labels and alt text for icon buttons, offers customizable high-contrast color modes, and allows instant font scaling.

Motor & Navigation Support: Overrides strict form timeouts that stress users with mobility limitations and optimizes keyboard navigation across complex multi-step menus and date pickers.

Health Literacy & Plain Language Toggle: Automatically scans the web page for dense medical jargon and confusing insurance terms (like deductible, benign, or hypertension), replacing or inline-defining them with clear, everyday language.

### How we built it

Extension Framework: Built using Manifest V3 to ensure modern security compliance, fast performance, and cross-browser compatibility (Chrome and Firefox).

DOM Manipulation & Accessibility Injection: JavaScript content scripts utilize dynamic MutationObserver instances to continuously audit single-page application (SPA) updates, injecting ARIA attributes and styling overrides on the fly.

Text Analysis Engine: Developed a lightweight DOM tree-walking algorithm paired with custom regular expression mappings to parse text nodes without breaking the underlying layout or form functions of the hospital's portal.

User Interface: Clean HTML/CSS popup menu providing one-click toggles for high-contrast mode, font size sliders, and feature switches.

### Challenges we ran into

Dynamic Web Apps (SPAs): Modern patient portals frequently re-render DOM elements dynamically. Ensuring our ARIA injection and text simplifiers re-ran without causing lag or infinite re-render loops required careful use of mutation observers and debouncing.

Preserving Functional Layouts: Overriding inline styles for high contrast and font scaling without breaking responsive grid layouts or hidden form fields was a tricky CSS exercise.

Balancing Medical Accuracy with Simplicity: Simplifying medical terminology requires extreme accuracy. We had to carefully curate dictionary definitions so terms remained medically accurate while remaining simple enough for a non-expert.

### Accomplishments that we're proud of

Zero Backend Requirement: We succeeded in making AccessMed 100% client-side, meaning it works immediately on third-party sites without needing hospital IT departments to modify their code or APIs.

Seamless Real-Time Parsing: Achieving smooth DOM text node replacement for plain-language definitions without visible page flicker or UI disruption.

Universal Impact: Creating a lightweight solution that solves visual, motor, and cognitive barriers simultaneously in a single tool.

### What we learned

Deepened our understanding of WCAG 2.1 guidelines and how critical programmatic aria-labels are for screen reader users.

Learned the nuances of working with Manifest V3 service workers and content script isolation.

Gained valuable insight into health literacy challenges and how design choices directly impact patient outcomes.

### What's next for AccessMed

AI-Powered Translation & Summarization: Integrate a lightweight local AI model or LLM API to summarize complex multi-page PDF medical records into 3 bullet points.

Voice Command Suite: Add Web Speech API capabilities so users with severe motor impairments can navigate portals entirely hands-free using voice commands like "Read lab results" or "Click messages."

Localized Multilingual Support: Expand the Plain Language engine to automatically translate medical summaries into multiple languages for non-native English speakers.

---

<a id="project-medvoice-koway0"></a>
## 46. MedVoice

- **Devpost:** [MedVoice](https://devpost.com/software/medvoice-koway0)
- **Crawl ID:** `medvoice-koway0`
- **Submitted to:** HackGwinnett 6.0
- **Built with:** html5, javascript

### Team

- [A Nemani](https://devpost.com/a-m-nemani17)

### Project links

- [github.com/an17-m/workshop](https://github.com/an17-m/workshop)

### Technology references

- [html5](https://devpost.com/software/built-with/html5)
- [javascript](https://devpost.com/software/built-with/javascript)

### Project description

### Inspiration

Watching a friend's grandmother struggle with daily medication management and lose her independence to reliance on others inspired MedVoice. No one should have to compromise their autonomy just to read a prescription label safely, which sparked our mission to build a barrier-free digital assistant.

### What it does

MedVoice turns any smartphone camera into a talking pharmacist for blind, low-vision, and hard-of-seeing users. By combining real-time OCR label scanning, slow-paced automated voice readouts, and universal physical controls (where any keystroke triggers the next step), MedVoice ensures patients can independently scan prescription bottles, verify dosages, and track their daily schedules safely.

### How we built it

The app is built as a single, ultra-fast web application using HTML5, Tailwind CSS (via CDN), and pure JavaScript (ES6+). It leverages native browser APIs:

navigator.mediaDevices.getUserMedia for live camera vision feed and bounding reticles.

window.speechSynthesis with optimized slow-paced pacing (rate: 0.75) for comprehensive accessibility readouts.

Custom Web Audio API sound synthesizers for tactile auditory feedback.

### Challenges we ran into

Designing an interface that remains fully usable without relying strictly on eyesight or precise touchscreen taps was a major design challenge. We solved this by implementing a Universal Key Control system—allowing users to press any physical key on their keyboard to advance prompts or trigger actions—alongside automatic audio indexing for all screen options.

### Accomplishments that we're proud of

Successfully engineering a zero-dependency, single-file accessible web app that runs instantly in any browser.

Designing an empathetic user experience specifically tuned for blind and elderly users with high-contrast elements, tactile Peter Tarka-inspired sculptural cards, and deliberate audio pacing.

Translating a deeply personal inspiration story into a functional, life-enhancing prototype.

### What we learned

We gained profound insights into inclusive design principles, learning how critical auditory cues, predictable menu structures, and robust keyboard navigation are for making healthcare technology genuinely accessible to everyone.

### What's next for MedVoice

Integrating advanced machine learning OCR models (such as Tesseract.js or cloud vision APIs) for offline prescription parsing.

Adding automated push notifications and caregiver alert summaries.

Expanding multi-language voice support to serve diverse communities globally.

---

<a id="project-carenav-2zymdw"></a>
## 47. CareNav

- **Devpost:** [CareNav](https://devpost.com/software/carenav-2zymdw)
- **Crawl ID:** `carenav-2zymdw`
- **Submitted to:** HackGwinnett 6.0
- **Built with:** css, html, javascript

### Team

- [Kevin Hsia](https://devpost.com/kevinhsia2010)
- [Jacob Shin](https://devpost.com/ijacobshin12)
- [Basil George Eldhose](https://devpost.com/basilgeorgeeldhose27)

### Project links

- [github.com/kevinhsia2010-oss/CareNav/tree/main](https://github.com/kevinhsia2010-oss/CareNav/tree/main)

### Images

- [Image 1](https://d112y698adiu2z.cloudfront.net/photos/production/software_photos/005/765/251/datas/original.png)
- [Image 2](https://d112y698adiu2z.cloudfront.net/photos/production/software_photos/005/765/252/datas/original.png)
- [Image 3](https://d112y698adiu2z.cloudfront.net/photos/production/software_photos/005/765/253/datas/original.png)
- [Image 4](https://d112y698adiu2z.cloudfront.net/photos/production/software_photos/005/765/254/datas/original.png)
- [Image 5](https://d112y698adiu2z.cloudfront.net/photos/production/software_photos/005/765/255/datas/original.png)
- [Image 6](https://d112y698adiu2z.cloudfront.net/photos/production/software_photos/005/765/257/datas/original.png)
- [Image 7](https://d112y698adiu2z.cloudfront.net/photos/production/software_photos/005/765/256/datas/original.png)
- [Image 8](https://d112y698adiu2z.cloudfront.net/photos/production/software_photos/005/765/258/datas/original.png)

### Technology references

- [css](https://devpost.com/software/built-with/css)
- [html](https://devpost.com/software/built-with/html)
- [javascript](https://devpost.com/software/built-with/javascript)

### Project description

### Inspiration

To help students and parents receive the care they need.

### What it does

Helps children and parents receive care.

### How we built it

Used Gemini for the code.

### Challenges we ran into

Many different saving issues that we ran into, and had to prompt it multiple times.

### Accomplishments that we're proud of

The overall product that we made.

### What we learned

AI is unpredictable when coding.

### What's next for CareNav

Additional improvements and more accommodations, such as signing up. Fine tuning current accommodations to ensure customer satisfaction.

---

<a id="project-medical-care-voice-navigator"></a>
## 48. Medical Care Voice Navigator

- **Devpost:** [Medical Care Voice Navigator](https://devpost.com/software/medical-care-voice-navigator)
- **Crawl ID:** `medical-care-voice-navigator`
- **Submitted to:** HackGwinnett 6.0
- **Built with:** cluade, kero

### Team

- [senseiwoo22 Miranda Reyes](https://devpost.com/senseiwoo22)
- [giasfclflbrehber](https://devpost.com/giasfclflbrehber)
- [seb123ser123456-art Miranda-Reyes](https://devpost.com/seb123ser123456-art)

### Project links

- [github.com/giasfclflbrehber/HACKGWINNETT](https://github.com/giasfclflbrehber/HACKGWINNETT/)

### Images

- [Image 1](https://d112y698adiu2z.cloudfront.net/photos/production/software_photos/005/765/338/datas/original.png)
- [Image 2](https://d112y698adiu2z.cloudfront.net/photos/production/software_photos/005/765/416/datas/original.png)

### Project description

### Inspiration

Medicare is too confusing for people with disabilities, so we wanted to build a simple voice tool to help.

### What it does

It answers questions, tracks deadlines, and explains health info out loud using your voice.

### How we built it

We built it using Python, speech recognition libraries, and MedlinePlus.

### Challenges we ran into

Dealing with broken Python installations, conflicting versions, and terminal errors was really difficult.

### Accomplishments that we're proud of

We successfully built a working voice-controlled app that makes a tough system accessible.

### What we learned

We learned how to use VS Code, manage virtual environments, and solve error messages.

### What's next for Medical Care Voice Navigator

We want to add deadline reminders, more health conditions, and get a doctor to review the content.

---

<a id="project-wayfind-1nd92m"></a>
## 49. Wayfind

- **Devpost:** [Wayfind](https://devpost.com/software/wayfind-1nd92m)
- **Crawl ID:** `wayfind-1nd92m`
- **Submitted to:** HackGwinnett 6.0
- **Built with:** ai

### Team

- [Yiming chen](https://devpost.com/techkid1126)

### Project links

- [yiming-202.github.io/Wayfind](https://yiming-202.github.io/Wayfind/)

### Images

- [Image 1](https://d112y698adiu2z.cloudfront.net/photos/production/software_photos/005/765/250/datas/original.png)

### Project description

### Inspiration

*No details provided in the crawl.*

### What it does

*No details provided in the crawl.*

### How we built it

*No details provided in the crawl.*

### Challenges we ran into

*No details provided in the crawl.*

### Accomplishments that we're proud of

*No details provided in the crawl.*

### What we learned

I learnd how to used github

### What's next for Wayfind

*No details provided in the crawl.*

---

<a id="project-the-doctor-decoder"></a>
## 50. The Doctor Decoder

- **Devpost:** [The Doctor Decoder](https://devpost.com/software/the-doctor-decoder)
- **Crawl ID:** `the-doctor-decoder`
- **Submitted to:** HackGwinnett 6.0
- **Built with:** ai, html, no

### Team

- [eileenarehman-work Rehman](https://devpost.com/eileenarehman-work)

### Project links

- [eileenarehman-work.github.io/The-Doctor-Decoder-eileen-rehman-/index.html](https://eileenarehman-work.github.io/The-Doctor-Decoder-eileen-rehman-/index.html)

### Images

- [Image 1](https://d112y698adiu2z.cloudfront.net/photos/production/software_photos/005/765/303/datas/original.png)
- [Image 2](https://d112y698adiu2z.cloudfront.net/photos/production/software_photos/005/765/314/datas/original.png)

### Technology references

- [html](https://devpost.com/software/built-with/html)

### Project description

- medications

- intro page

### Inspiration

Doctor trips can be stressful and we don't need added stress.

### What it does

Gives simple definitions of top 5 medications

### How I built it

Using HTML

### Challenges I ran into

First time using HTML so I needed to go between tutorials and code.

### Accomplishments that I'm proud of

First HTML project and no AI

### What I learned

How to use HTML

### What's next for The Doctor Decoder

More medications and possibly diagnoses

VIDEO WAS EMAILED.

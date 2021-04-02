# Connect All

Connect All is an application developed to help the disabled communicate and live life normally. This was developed as a term project for ET60029 (TECHNOLOGY FOR SPECIAL NEEDS EDUCATION) and is an umbrella service for multiple aids. 

You may use this app in 3 ways -
- Deployed with zeit - http://web.jvank.now.sh . You may use this app to access all facilities.

## Sign Language to Text and more ...

Sign language gives voice to the mute and is the sound for the deaf. Using deep neural networks, we convert sign language to text, aiding those unable to comprehend sign language.

![Sign Language Example](https://raw.githubusercontent.com/thealphadollar/T4SNE-Connnect-All/master/backend/app/main/utils/toSignTranslator/ISL_Gifs/shall%20we%20go%20together%20tommorow.gif)

## Instant Message 4 all

Real time lag-free chat is made possible by hacks at socket level.To aid the specially-abled, speech-to-text and text-to-speech is also used on the fly. Technology stack used for this is socket.io, google cloud speech API.

![Instant Message 4 all](https://raw.githubusercontent.com/thealphadollar/T4SNE-Connnect-All/master/all_inputs/im4all_example/im4all.png)

## Book Narration

The workflow for a seamless narration of books begins by obtaining text using combination of pdf-parsing and OCR. The narration audios generated for each page is stitched together. The technology stack consists of Azure services for OCR and Audio. Apache Tika and PyPDF2 is used for parsing pdfs.

![Book Narration](https://raw.githubusercontent.com/thealphadollar/T4SNE-Connnect-All/master/all_inputs/books/book_ex_website.png)

## Note Taking

The workflow starts with image - preprocessing and identification of skewedness and inversion of text. The text is extracted along with exact position and font size. The text is then intelligently parsed for clubbing various parts of the note under a heading / sub-heading or bullets and numbering.

![Note Example](https://raw.githubusercontent.com/thealphadollar/T4SNE-Connnect-All/master/all_inputs/notes/note_ex.png)

It then appropriately narrates the various sections of the note. The technology stack consists of Azure Vision service, OpenCV and Azure Speech service.

## Backend

To run the backend

```shell
cd /backend
pipenv shell --three    #only the first time
python3 manage.py run
```
## Frontend

To deploy the frontend on zeit

```shell
cd /docs/web
npm i -g now    #intall now cli
now login
now
```

Open the respective link to view the rest API and test it.

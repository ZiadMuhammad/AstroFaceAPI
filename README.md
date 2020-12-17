# AstroFaceAPI ♒️
I created this API just as a little experiment to see if deep learning could detect your zodiac sign from your image! The model got trained on a dataset that I collected on my own. The dataset consisted of photos of celebrities of different zodiac signs.

# How to use this API?
First of all, you need to download Keras, TensorFlow, and flask if you don't already have them.

-To download TensorFlow:

```bash
  pip install tensorflow
```

-To download Keras:


```bash
  pip install keras
```

-To download Flask:


```bash
  pip install flask
```

Then clone this repository and through the terminal go to the repository's directory and run the server:

```bash
  python3 app.py
```

To use this API, you can use your browser and navigate to http://localhost:5000 and, from there, you can upload your image and see if the model could detect your zodiac sign! You can also send a POST request to http://localhost:5000/predict with your image's link in the request's body.

Example POST Request's body:

```json
  {
    "image_link": "https://www.gstatic.com/tv/thumb/persons/82335/82335_v9_bb.jpg"
  }
```

Response:
```
  You look like a Taurus
```

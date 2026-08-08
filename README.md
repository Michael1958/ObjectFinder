# ObjectFinder

**Find images on your computer by subject, right from your browser.**

ObjectFinder lets you search a folder on your computer for images that contain a specific subject. You can upload a photo and pick the subject, or simply type a short description of what to find. Everything runs inside your browser, so your images never leave your computer.

### Open the app
[https://michael1958.github.io/ObjectFinder/](https://michael1958.github.io/ObjectFinder/)

---

## What you can do

- Upload an image and select a subject (a person, an animal, or an object), then search a folder and all its subfolders for matching images.
- Or type a short description, for example "black cat", "black and white dog", or "a goose", and search without uploading anything.
- For a person, the app matches by face, so it finds the same individual when the face is clearly visible.
- View any result in a large preview, or download a copy.

---

## Before you start

- Use **Microsoft Edge or Google Chrome on a desktop or laptop**. The folder search is not available on phones, tablets, Firefox, or Safari.
- You need an **internet connection the first time you run a search**. The app downloads its recognition models once, then keeps them for reuse, so later searches work faster.
- The **first search takes about a minute** while those models download. This is a one-time step.
- **Your privacy is protected.** Images are processed only on your computer and are never uploaded anywhere.

---

## How to use it, in four steps

1. Open the link and either upload an image or type a description.
2. If you uploaded an image, choose the subject you want to find.
3. Choose the folder on your computer to search.
4. Review the ranked results, then adjust the similarity slider if you want fewer or more matches.

If nothing appears on the first try, please wait a moment for the models to finish downloading, then search again.

---

## How it works

ObjectFinder runs entirely in your browser using three AI models that load automatically the first time they are needed:

| Search type | What it matches | Model used |
| --- | --- | --- |
| Object or animal (from an image) | The same kind of subject | Object detection plus image similarity |
| Person (from an image) | The same individual, by face | Face recognition |
| Description (typed text) | Images matching your words | Text to image similarity |

- **Colors and simple descriptions** work well, for example "black cat" or "brown horse".
- **Common animals** such as cat, dog, bird, and horse are detected precisely. Less common ones, for example a goose or an eagle, use a looser whole-image match.
- **People** are matched by face when the face is clearly visible, so a different person will not match.

---

## Privacy

All processing happens locally in your browser. Your images and the folder you choose are never uploaded to any server. The only network activity is a one-time download of the recognition models from a public code library, after which they are cached for offline reuse.

---

## Known limitations

- Desktop **Microsoft Edge or Chrome only**, because the folder picker needs the File System Access API.
- Matching an exact individual applies to **people (by face)**, not to specific animals or objects.
- Face matching needs a **clearly visible face**. Profiles, blurry, tiny, or covered faces may be missed.
- For speed, the app indexes the first 400 images in a folder.
- Supported image formats: JPG, JPEG, PNG, WEBP, GIF, BMP.

---

*Created by Michael Gerontides*

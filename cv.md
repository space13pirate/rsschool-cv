# Anastasia Cheremisova

<div id="header" align="left">
  <img src="https://i.ibb.co/NZbH7SS/rsschool-cv.jpg" width="150"/>
</div>

---

## Contact Information

| Contact Type  |       Details
----------------|:--------------------------:
**Email**       |north13anastasia@gmail.com
**Phone**       |+7 (927) 044-74-75
**Discord**     |space13pirate

---

## About Me

:ledger: I am a student at Kazan State Power Engineering University (KSPEU).

:ninja: Currently, I explore the vast universe of programming as a space pirate, aiming to become a programming ninja...

:footprints: My journey in programming is fuelled by a relentless pursuit of knowledge and a passion for developing innovative solutions.

---

## Skills

### Programming Languages
* **Python** – experienced in application development, data handling, and machine learning. Developed a web application for emotion recognition using neural networks.
* **PHP** – developed a pet project for airport administration.
* **JavaScript**, **HTML**, **CSS** – used for web development.
* **Dart (Flutter)** – used for developing cross-platform mobile applications.
* **Java** – used for mobile application development.
* **C#** and **C++** – beginner level proficiency.

### Frameworks
* **Flask** – used for creating Python-based web applications.
* **React** – utilized for building user interfaces.
* **Flutter** – employed for creating efficient and aesthetically pleasing cross-platform mobile applications.

### Development Tools
* **Git** – proficient in using Git for version control.

### Methodologies
* **Agile** and **Scrum** – methodologies followed during project development, ensuring efficient and flexible project management.

---

### Code Examples

* An example of solving a problem from [Codewars](https://www.codewars.com/ "Go to Codewars"):

```javascript
function multiply(a, b){
  return a * b;
}
```

* Python function from my *EmoDetect* project:

```python
def detect_face(frame):
  """
  Определение ключевых точек на лице и возвращение координат (не используется в предсказании модели, но в визуализации)
  """
  # Предварительно обученная модель классификатора каскадов
  cascPath = 'Models/face_landmarks.dat'        # Путь к предварительно обученной модели классификатора каскадов
  faceCascade = cv2.CascadeClassifier(cascPath) # Загрузка классификатора каскадов

  # Конвертация изображения BGR -> Gray
  gray = cv2.cvtColor(frame, cv2.COLOR_BGR2GRAY)

  # Обнаружение лиц на изображении
  detected_faces = faceCascade.detectMultiScale(gray, scaleFactor=1.1, minNeighbors=6,
                                                minSize=(shape_x, shape_y),
                                                flags=cv2.CASCADE_SCALE_IMAGE)
  coord = []  # Координаты обнаруженных лиц

  for x, y, w, h in detected_faces:
    if w > 100: # Если ширина обнаруженного лица больше 100
      sub_img = frame[y:y + h, x:x + w]   # Квадрат вокруг ключевых точек на лице
      cv2.rectangle(frame, (x, y), (x + w, y + h), (0, 255, 255), 1)  # Обвести лицо прямоугольником
      coord.append([x, y, w, h])          # Добавление координат лица в список

  return gray, detected_faces, coord
```

---

## Work Experience

### Academic Projects

* [Аэропортал: от входа до взлёта]([адрес](https://github.com/space13pirate/airport_admin) "Go to github.com/space13pirate/airport_admin")
  + **Technology:** PHP
  + **Description:** Developed a management system for airport operations as a pet project.

* **EmoDetect**
    + **Note:** The source code for EmoDetect is not currently available for public viewing as it is part of a graduation thesis and subject to confidentiality requirements.
    + **Technologies:** Python, Flask
    + **Description:** Created a web application that uses neural networks to recognize human emotions from audio and video data.
    + **Skills:** Python, machine learning, web application development.

---

## Education

:heavy_check_mark: Bachelor's Degree from Kazan State Power Engineering University (KSPEU)
* **GPA:** 4.6

### Professional Development and Training

:heavy_check_mark: **DevOps Engineer**
* **Institution:** Kazan State Power Engineering University (KSPEU)
* **Description:** Diploma in professional retraining in DevOps engineering.

:heavy_check_mark: **Software Developer**
* **Institution:** Innopolis University
* **Description:** Diploma in professional retraining obtained after completing a program on the fundamentals of software development management and new production technologies.

:heavy_check_mark: **Startup: Commercialization of Scientific Research Results Using Mathematical Modeling**
* **Institution:** Kazan State Power Engineering University (KSPEU)
* **Description:** Additional educational program аocused on commercializing scientific achievements through startup initiatives and mathematical modeling.

:heavy_check_mark: **Software Engineering: IT Leaders of the Future**
* **Institution:** Innopolis University
* **Status:** Currently enrolled in this professional retraining program.
  

:heavy_check_mark: **JavaScript/Front-end. Pre-school**
* **Institution:** RS School
* **Description:** Currently enrolled in a preparatory course focusing on JavaScript and front-end development fundamentals.

---

## Language Proficiency

* **Russian** – Native speaker
* **English**
  + **Level:** B2 (Upper-Intermediate)
  + **Experience:**  Successfully defended a project in English during a course at Innopolis University, which included both presentation and discussion phases in English.

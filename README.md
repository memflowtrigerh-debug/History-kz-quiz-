# History-kz-quiz-
&lt;div class="admin">   Админ программы: &lt;b>Якубахунов Шахрух&lt;/b>&lt;br>   Руководитель: &lt;b>Гульмира Зиявдуновна&lt;/b> &lt;/div>  &lt;h1>Интерактивный квиз: История Казахстана — 9 класс&lt;/h1>  &lt;div class="description">   Добро пожаловать! Здесь интерактивный онлайн-квиз по истории Казахстана для 9 класса. Проверяйте свои знания и учитесь с интересом! &lt;/div>
<!DOCTYPE html>
<html lang="ru">
<head>
<meta charset="UTF-8">
<title>История Казахстана — 9 класс</title>

<style>
body {
  font-family: Arial, sans-serif;
  background: linear-gradient(135deg,#00c6ff,#0072ff);
  padding: 40px;
}
.quiz {
  max-width: 750px;
  margin: auto;
  background: #ffffff;
  padding: 25px;
  border-radius: 15px;
  box-shadow: 0 10px 25px rgba(0,0,0,0.25);
}
.admin {
  text-align: center;
  font-size: 15px;
  color: #444;
  margin-bottom: 15px;
}
h1 {
  text-align: center;
}
.question {
  margin-bottom: 20px;
}
label {
  display: block;
  margin: 6px 0;
  cursor: pointer;
}
button {
  width: 100%;
  padding: 14px;
  font-size: 18px;
  border: none;
  border-radius: 10px;
  background: #0072ff;
  color: #fff;
  cursor: pointer;
}
button:hover {
  background: #005bd1;
}
#result {
  margin-top: 20px;
  font-size: 20px;
  text-align: center;
  font-weight: bold;
}
</style>
</head>

<body>

<div class="quiz">

  <!-- ТЕКСТ В НАЧАЛЕ -->
  <div class="admin">
    Админ программы: <b>Якубахунов Шахрух</b><br>
    Руководитель: <b>Гульмира Зиявдуновна</b>
  </div>

  <h1>История Казахстана (9 класс)</h1>

  <div class="question">
    <p>1. В каком году было образовано Казахское ханство?</p>
    <label><input type="radio" name="q1">1456</label>
    <label><input type="radio" name="q1" id="q1">1465–1466</label>
    <label><input type="radio" name="q1">1500</label>
  </div>

  <div class="question">
    <p>2. Кто были основателями Казахского ханства?</p>
    <label><input type="radio" name="q2" id="q2">Керей и Жанибек</label>
    <label><input type="radio" name="q2">Абылай и Кенесары</label>
    <label><input type="radio" name="q2">Касым и Тауке</label>
  </div>

  <div class="question">
    <p>3. Как назывался свод законов при Тауке хане?</p>
    <label><input type="radio" name="q3">Алтын заң</label>
    <label><input type="radio" name="q3" id="q3">Жеты Жаргы</label>
    <label><input type="radio" name="q3">Кодекс степи</label>
  </div>

  <div class="question">
    <p>4. Что стало причиной восстания 1916 года?</p>
    <label><input type="radio" name="q4">Коллективизация</label>
    <label><input type="radio" name="q4" id="q4">Призыв на тыловые работы</label>
    <label><input type="radio" name="q4">Распад СССР</label>
  </div>

  <div class="question">
    <p>5. В каком году был закрыт Семипалатинский ядерный полигон?</p>
    <label><input type="radio" name="q5">1989</label>
    <label><input type="radio" name="q5" id="q5">1991</label>
    <label><input type="radio" name="q5">1995</label>
  </div>

  <div class="question">
    <p>6. Какое движение выступало против ядерных испытаний?</p>
    <label><input type="radio" name="q6">Алаш</label>
    <label><input type="radio" name="q6">Азат</label>
    <label><input type="radio" name="q6" id="q6">Невада – Семипалатинск</label>
  </div>

  <button onclick="check()">Проверить результат</button>
  <div id="result"></div>

</div>

<script>
function check() {
  let score = 0;
  if (q1.checked) score++;
  if (q2.checked) score++;
  if (q3.checked) score++;
  if (q4.checked) score++;
  if (q5.checked) score++;
  if (q6.checked) score++;

  let text = "Результат: " + score + " из 6<br>";
  if (score === 6) text += "🔥 Отлично!";
  else if (score >= 4) text += "👍 Хорошо";
  else text += "📘 Нужно повторить материал";

  document.getElementById("result").innerHTML = text;
}
</script>

</body>
</html>

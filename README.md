# 🌈 אנגלית בכיף! — מדריך הוספת תוכן

## מבנה הפרויקט

```
english-app/
├── index.html   ← האפליקציה עצמה (לא לגעת!)
├── data.js      ← כל התוכן — פה מוסיפים שיעורים!
└── README.md    ← המדריך הזה
```

## 🚀 הפעלה
פשוט לפתוח את `index.html` בדפדפן (Chrome / Safari / Firefox).  
לא צריך שרת, לא צריך התקנה.

---

## ➕ הוספת נושא מילים חדש

פתחו את `data.js` וחפשו את המערך `vocabTopics`.  
העתיקו בלוק קיים והוסיפו בסוף המערך (לפני הסוגר `]`):

```js
{
  id: 'sports',           // מזהה ייחודי (באנגלית, בלי רווחים)
  title: 'ספורט 🏅',       // שם הנושא (עברית + אמוג'י)
  emoji: '⚽',             // אמוג'י לכפתור
  color: '#FF5722',        // צבע (קוד HEX)
  words: [
    {en:'Soccer',  he:'כדורגל',  emoji:'⚽'},
    {en:'Swimming',he:'שחייה',   emoji:'🏊'},
    {en:'Tennis',  he:'טניס',    emoji:'🎾'},
    // ... עד 10 מילים מומלץ
  ]
},
```

✅ זהו! שמרו את הקובץ ורעננו את הדפדפן — הנושא יופיע אוטומטית.

---

## ➕ הוספת שיר / חרוז חדש

חפשו את המערך `songs` ב-`data.js`:

```js
{
  id: 'baa_baa',
  title: 'Baa Baa Black Sheep',
  emoji: '🐑',
  color: '#9C27B0',
  lines: [
    {text:'Baa baa black sheep,',    he:'מה, מה, כבשה שחורה'},
    {text:'Have you any wool?',      he:'?האם יש לך צמר'},
    {text:'Yes sir, yes sir,',       he:'כן אדוני, כן אדוני'},
    {text:'Three bags full!',        he:'!שלושה שקים מלאים'},
  ]
},
```

---

## ➕ הוספת שיעור דקדוק חדש

חפשו את המערך `grammarLessons`:

```js
{
  id: 'opposites',
  title: 'הפכים',
  emoji: '↔️',
  color: '#3F51B5',
  explanation: [
    {rule:'Big ↔ Small', example:'a big dog / a small cat', he:'גדול מול קטן'},
    {rule:'Hot ↔ Cold',  example:'hot soup / cold water',   he:'חם מול קר'},
  ],
  quiz: [
    {q:'Big ↔ ___', opts:['Small','Big','Tall','Heavy'], ans:'Small', emoji:'📦'},
    {q:'Hot ↔ ___',  opts:['Warm','Hot','Cold','Cool'],  ans:'Cold',  emoji:'🌡️'},
    // ... הוסיפו עד 8 שאלות
  ]
},
```

---

## ➕ הוספת משפטים לקבוצת משפטים

חפשו את `sentenceGroups` ב-`data.js`.  
כל קבוצה כוללת `sentences`. להוסיף שורה:

```js
{en:'I am excited!', he:'!אני נרגש/ת', emoji:'🤩', tip:'כשמתרגשים מאיזה דבר'},
```

---

## ➕ הוספת שאלות לחידון

חפשו `wordQuizPool` ב-`data.js`:

```js
{q:'מה זה? 🏀', opts:['Soccer','Tennis','Basketball','Baseball'], ans:'Basketball', emoji:'🏀'},
```

---

## 🎨 צבעים מומלצים לנושאים חדשים

| צבע       | HEX       |
|-----------|-----------|
| כחול שמיים | `#4FC3F7` |
| ירוק      | `#66BB6A` |
| כתום      | `#FFA726` |
| סגול      | `#AB47BC` |
| ורוד      | `#EC407A` |
| אדום      | `#FF7043` |
| ציאן      | `#26C6DA` |
| אינדיגו   | `#5C6BC0` |

---

## 💡 טיפים

- כדאי להוסיף בין 8–12 מילים לכל נושא
- האמוג'י חייב להתאים למילה בדיוק
- שמרו את `id` ייחודי (אחרת נושאים יתנגשו)
- אחרי שמירה: רענון הדפדפן (F5) — השינוי מיידי!

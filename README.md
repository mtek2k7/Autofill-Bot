# Autofill-Bot
**Autofill Bot** is a tool designed to automatically fill answers in forms or multiple-choice quizzes. Instead of manually selecting each option, the bot allows you to input answers in a single line and automatically fills the corresponding **radio buttons** or **checkboxes**.

## How It Works
### No.1
- Input key (contact me)
### No.2
- After inputing a key, bot ask "Enter URL - page (For example Google Form or other pages which have checkbox, radio):", you input a link which have checkbox, radio that you request bot mark on
- Next step, choosing a mode

  **1. Input String list (enter the number of string before entering string by string respectively).**  
  **2. Syntax:**   
| Prefix / Syntax               | Action                      | Description / Notes                                                                                  |
| ----------------------------- | --------------------------- | ---------------------------------------------------------------------------------------------------- |
| `checkbox:Label`              | Check a checkbox            | Finds the checkbox with the given label (exact or fuzzy match).                                      |
| `radio:Label`                 | Select a radio button       | Finds the radio button with the given label (exact or fuzzy match).                                  |
| `uncheck:Label`               | Uncheck a checkbox          | Only works for checkboxes.                                                                           |
| `!Label`                      | Shortcut for uncheck        | Only works for checkboxes.                                                                           |
| `(Label)`                     | Click a button              | Finds and clicks a button whose visible text matches the label. Supports English or other languages. |
| `click:Label` / `press:Label` | Click a button              | Directly click a button by its visible text on the page.                                             |
| No prefix                     | Check a checkbox by default | If no prefix is specified, the bot will try to find a checkbox or radio button.                      |

💡 Tip: Labels do not need to be exact. The bot supports fuzzy match and contains match.

  **3) Input One line, items separated by '/' (for example: a / b / !Subscribe / (Submit). like below:**
The bot accepts answers in a simple format such as:

*Mode 1 - how many option do you want to fill. For example: I wanna input 3 options -> Enter '3' -> Enter respectively:*   
```
 option 1  
 option 2  
 option 3
```
or   

*Mode 2 - enter instantly like below structure:*   
```
 option 1 / option 4 / option 5
```

**Example:**

If a question requires selecting:

* Option 1
* Option 4
* Option 5

You simply enter:

*Mode 1:*   
```
 option 1  
 option 2  
 option 3
```
or   

*Mode 2:*   
```
 option 1 / option 4 / option 5
``` 

After receiving this input, the bot will:

* Detect the corresponding options in the question
* Automatically select the correct **radio buttons** or **checkboxes** in the form
* Fill the answers according to the provided order
### No.3
- Login in: If your website require log in, you enter 'y'
- Enter username and password (note: If you log in on "Google account", please logging in manually)
### No.4
- How many times do you want the bot to run (integer >=1): bot will open a number of tab you enter.
- Run headless? (y/n): if you want bot to open chorme enter 'n'

## Benefits

* ⚡ **Faster** than manually selecting each answer
* 🤖 **Automates** the process of filling forms or quizzes
* ⏱ **Saves time** when working with many questions
* 📋 **Easy to use** with a simple input format

## Usage Tip

You can ask an AI or system to answer all multiple-choice questions and output the results in this format:

*Mode 1:*   
```
 option 1  
 option 2  
 option 3
```
or   

*Mode 2:*   
```
 option 1 / option 4 / option 5
``` 
Then paste that line into **Autofill Bot**, and it will quickly select the answers in the form for you.

# How to use
- First, click '<>Code' before clicking 'Download zip'
- Second, open file autofill_bot.exe in file Autofill-Bot-main.zip

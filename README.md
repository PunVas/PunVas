
## 🌐 Socials:
[![LinkedIn](https://img.shields.io/badge/LinkedIn-%230077B5.svg?logo=linkedin&logoColor=white)](https://linkedin.com/in/puneet-v-171885310)

# 💻 Tech Stack:
![C++](https://img.shields.io/badge/c++-%2300599C.svg?style=for-the-badge&logo=c%2B%2B&logoColor=white) ![C](https://img.shields.io/badge/c-%2300599C.svg?style=for-the-badge&logo=c&logoColor=white) ![Bash Script](https://img.shields.io/badge/bash_script-%23121011.svg?style=for-the-badge&logo=gnu-bash&logoColor=white) ![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54) ![TensorFlow](https://img.shields.io/badge/TensorFlow-%23FF6F00.svg?style=for-the-badge&logo=TensorFlow&logoColor=white) ![scikit-learn](https://img.shields.io/badge/scikit--learn-%23F7931E.svg?style=for-the-badge&logo=scikit-learn&logoColor=white) ![HTML5](https://img.shields.io/badge/html5-%23E34F26.svg?style=for-the-badge&logo=html5&logoColor=white) ![JavaScript](https://img.shields.io/badge/javascript-%23323330.svg?style=for-the-badge&logo=javascript&logoColor=%23F7DF1E) ![PHP](https://img.shields.io/badge/php-%23777BB4.svg?style=for-the-badge&logo=php&logoColor=white) ![MySQL](https://img.shields.io/badge/mysql-4479A1.svg?style=for-the-badge&logo=mysql&logoColor=white) ![NumPy](https://img.shields.io/badge/numpy-%23013243.svg?style=for-the-badge&logo=numpy&logoColor=white) ![FastAPI](https://img.shields.io/badge/FastAPI-005571?style=for-the-badge&logo=fastapi) ![GitHub Actions](https://img.shields.io/badge/github%20actions-%232671E5.svg?style=for-the-badge&logo=githubactions&logoColor=white)
# 📊 GitHub Stats:
![](https://github-readme-stats.vercel.app/api?username=PunVas&theme=tokyonight&hide_border=false&include_all_commits=false&count_private=true)<br/>
![](https://github-readme-streak-stats.herokuapp.com/?user=PunVas&theme=tokyonight&hide_border=false)<br/>
![](https://github-readme-stats.vercel.app/api/top-langs/?username=PunVas&theme=tokyonight&hide_border=false&include_all_commits=false&count_private=true&layout=compact)

## 🏆 GitHub Trophies
![](https://github-profile-trophy.vercel.app/?username=PunVas&theme=tokyonight&no-frame=false&no-bg=false&margin-w=4)


```asm
section .data
    life db "chai + college + coding + shinchan", 0

section .text
    global _start

_start:
    ; Print the meaning of life
    mov rax, 1
    mov rdi, 1
    mov rsi, life
    mov rdx, 34
    syscall

    mov rax, 60
    xor rdi, rdi
    syscall
```

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Read Cookie XYZ</title>
    <style>
        /* CSS Rule: This will trigger a request to read_cookie.php when the #cookie-reader element is present */
        /* Note: Using background-image is often less intrusive than 'content' for pseudo-elements if you don't need the content itself */
        #cookie-reader {
            /* This URL triggers the PHP script to read the cookie */
            background-image: url('read_cookie.php?action=read-xyz');
            /* Make the element invisible if you don't need it visible */
            position: absolute;
            left: -9999px;
        }

        /* Optional: Style an element to display the cookie value if needed */
        .cookie-display {
            margin-top: 20px;
            padding: 10px;
            border: 1px solid #ccc;
            background-color: #f9f9f9;
        }
    </style>
</head>
<body>

    <h1>Reading Cookie Example</h1>
    <p>This page demonstrates reading a cookie named 'xyz' using CSS to trigger a PHP script.</p>

    <!-- This hidden element triggers the CSS rule that fetches the PHP script -->
    <div id="cookie-reader" aria-hidden="true"></div>

    <!-- Optional: Element to display the cookie value, populated by the PHP script -->
    <div class="cookie-display">
        <strong>Cookie 'xyz' Value (as seen by PHP on load):</strong>
        <?php
        // This PHP block runs *once* when the main page loads,
        // showing the value if it existed *at that moment*.
        if (isset($_COOKIE['xyz'])) {
            echo htmlspecialchars($_COOKIE['xyz']); // Use htmlspecialchars to prevent XSS
        } else {
            echo 'Cookie "xyz" not found or not set.';
        }
        ?>
    </div>

    <!-- Optional: Link to set the cookie for testing -->
    <p><a href="read_cookie.php?action=set-xyz&value=test_value_<?php echo time(); ?>">Set Cookie 'xyz' to a test value</a> (This will trigger the PHP script directly)</p>

</body>
</html>

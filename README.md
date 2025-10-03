<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>flow1.java Code</title>
    <style>
        body {
            font-family: Consolas, monospace;
            background-color: #f5f5f5;
            padding: 20px;
        }
        pre {
            background-color: #272822;
            color: #f8f8f2;
            padding: 20px;
            border-radius: 8px;
            overflow-x: auto;
        }
        button {
            margin-top: 10px;
            padding: 8px 12px;
            background-color: #4CAF50;
            color: white;
            border: none;
            border-radius: 5px;
            cursor: pointer;
        }
        button:hover {
            background-color: #45a049;
        }
    </style>
</head>
<body>

<h2>flow1.java</h2>
<pre id="code">
import javax.swing.*;
import java.awt.*;

public class flow1 extends JFrame {
    JButton b1, b2, b3;

    public flow1() {
        FlowLayout f1 = new FlowLayout(FlowLayout.RIGHT, 100, 50);
        setLayout(f1);
        b1 = new JButton("1");
        b2 = new JButton("2");
        b3 = new JButton("3");
        add(b1);
        add(b2);
        add(b3);

        setSize(400, 400);
        setDefaultCloseOperation(JFrame.EXIT_ON_CLOSE);
        setVisible(true);
    }

    public static void main(String args[]) {
        new flow1();
    }
}
</pre>

<button onclick="copyCode()">Copy Code</button>

<script>
function copyCode() {
    const code = document.getElementById("code").innerText;
    navigator.clipboard.writeText(code).then(() => {
        alert("Code copied to clipboard!");
    });
}
</script>

</body>
</html>

<h1>Eu sou o Lucas Feliciano!</h1>
import javax.swing.*;
import java.awt.*;

public class MovingEmoji extends JPanel implements Runnable {
    private int x = 0;
    private int direction = 1;

    public MovingEmoji() {
        setPreferredSize(new Dimension(800, 200));
        Thread animationThread = new Thread(this);
        animationThread.start();
    }

    @Override
    protected void paintComponent(Graphics g) {
        super.paintComponent(g);
        // Desenhe o emoji da mão aqui (substitua com um emoji ou desenho de mão)
        g.setFont(new Font("SansSerif", Font.PLAIN, 100));
        g.drawString("👋", x, 100);
    }

    @Override
    public void run() {
        while (true) {
            x += direction;
            if (x >= getWidth() - 100 || x <= 0) {
                direction *= -1;
            }
            repaint();
            try {
                Thread.sleep(10);
            } catch (InterruptedException e) {
                e.printStackTrace();
            }
        }
    }

    public static void main(String[] args) {
        JFrame frame = new JFrame("Moving Emoji");
        frame.setDefaultCloseOperation(JFrame.EXIT_ON_CLOSE);
        frame.add(new MovingEmoji());
        frame.pack();
        frame.setLocationRelativeTo(null);
        frame.setVisible(true);
    }
}

<br>
<p>- Trabalho na empresa Smartfit</p>
<p>- Me encontro no último semestre da faculdade de Análise e Desenvolvimento de Sistemas</p>
<p>- Tenho 27 anos de idade</p>
<p>- Amo trabalhar com programação</p>
<br>
<p align="left">

<img width="530em" src="https://github-readme-stats.vercel.app/api?username=lucasfelician0&show_icons=true&theme=onedark" alt="lucasfelician0's stats"/>

<p>
    <img width="530em" src="https://github-readme-stats.vercel.app/api/top-langs/?username=lucasfelician0&layout=compact" alt="lucasfelician0's top languages"/>
    <br> 
    <img align="center" alt="RUBY" src="https://img.shields.io/badge/Ruby-CC342D?style=for-the-badge&logo=ruby&logoColor=white">
    <img align="center" alt="PYTHON" src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white">
    <img align="center" alt="HTML5" src="https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white">
    <img align="center" alt="JAVASCRIPT" src="https://img.shields.io/badge/JavaScript-323330?style=for-the-badge&logo=javascript&logoColor=F7DF1E">
</p>




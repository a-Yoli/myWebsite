+++
date = '2024-11-13T15:33:38+01:00'
draft = false
title = 'Setting Up the Website'
category = ['Course: Interaction in Virtual and Augmented Reality 2024/2025']
+++

To set up this website I used [Hugo](https://gohugo.io) as recommended within our course. The process was generally straightforward, but I noticed that the [Quick start tutorial](https://gohugo.io/getting-started/quick-start/) asks for Hugo v0.128.0. The version which I installed via the dnf software package manager as recommended by [Hugo's linux nstallation guide](https://gohugo.io/installation/linux/) (my operating system is Fedora) was much lower (v0.111...). While this version might have sufficed to create a Hugo website, I also needed a newer version for the theme I wanted to use ([Hugo Theme Stack](https://themes.gohugo.io/themes/hugo-theme-stack/#documentation)) So without using the snap package manager, my only option was to build it from source. After I did that, I could finally use the theme I wanted.

With that I could continue creating my page. Unfortunately, my posts wouldn't show up and if you wonder, if I just forgot to add the ```-D``` flag to the ```hugo server``` command, I have to disappoint you. So I turned to the internet as usual when I have a problem with software and found the solution in the [hugo forums](https://discourse.gohugo.io/t/new-to-hugo-content-posts-do-not-display-anything/28298): the automatically created folder structure named the folder for posts 'posts' but mytheme asked for the name to be 'post'. With that I finally had my working website. I plan on editing the website later on to make it more visually pleasing but for now it has all that I need.



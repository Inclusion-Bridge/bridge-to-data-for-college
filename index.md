---
layout: home
title: Home
nav_order: 1
nav_exclude: false
permalink: index.html
seo:
  type: Course
  name: Data 8 Spring 2024
---

# Data 8: Foundations of Data Science

{: .mb-2 }
InclusionBridge, Bridge to Data Fundamentals (Mercy University) 2024
{: .mb-2 .fs-6 .text-grey-dk-000 }

[Lecture Zoom Link](https://us06web.zoom.us/my/ttogun?pwd=bGsxeU1uN0F0ZHVTQ1NBTWVWNUNEdz09){: .btn .btn-blue}

## Let us start your Data Science Journey together

**Acknowledgements**

This course is based on Data 8, titled "The Foundations of Data Science," a course taught to first-year students at UC Berkeley. All course materials, including the textbook and assignments, are provided free of charge online under a Creative Commons license. The textbook, "[Computational and Inferential Thinking: The Foundations of Data Science](https://inferentialthinking.com/chapters/intro.html)," is an online resource featuring Jupyter notebooks and publicly accessible data sets used in all the examples. The course materials comprise Embedded Demo, Lab, and Homework Notebooks, as well as references, all sourced from the public [Data8 repository](https://github.com/data-8). Students are encouraged to visit the [official Data8 website](https://www.data8.org/) for additional resources, including complete lecture videos and PowerPoint presentations.

{% assign announcements = site.announcements | reverse %}
{% for announcement in announcements %}
{{ announcement }}
{% endfor %}

{% assign mods = site.modules | where: 'class', 'CollegeAdvantage' %}
{% for module in mods %}
{{ module }}
{% endfor %}

<
<br />

<button class="js-toggle-dark-mode dm-btn btn">Toggle Dark Mode</button>

<script src="assets/darkmode.js"></script>
<script>
  const toggleDarkMode = document.querySelector('.js-toggle-dark-mode');

  jtd.addEvent(toggleDarkMode, 'click', function(){
    if (jtd.getTheme() === 'custom_dark') {
      jtd.setTheme('light');
      localStorage.setItem("darkMode", 0);
      toggleDarkMode.innerHTML = "Toggle Dark Mode";
      toggleDarkMode.classList.add('dm-btn');
        toggleDarkMode.classList.remove('dm-dark-btn');
    } else {
      jtd.setTheme('custom_dark');
      localStorage.setItem("darkMode", 1);
      toggleDarkMode.innerHTML = "Return to the Light";
      toggleDarkMode.classList.add('dm-dark-btn');
      toggleDarkMode.classList.remove('dm-btn');
    }
  });

    window.addEventListener("DOMContentLoaded", (event) => {
      onLoad();
  });
</script>

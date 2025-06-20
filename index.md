---
layout: default
title: Home
permalink: /
---

# Jason Terrance Wells, MD
## MBA Candidate & Computer Science Student

Welcome to my personal website! I am a dedicated medical professional with extensive experience in General Surgery, currently expanding my expertise as an **MBA Candidate at Carnegie Mellon University** and pursuing a **B.S. in Computer Science at the University of Colorado, Boulder**.

My journey has provided me with a unique perspective on problem-solving, critical thinking, and leadership. I am now channeling these skills, combined with a passion for technology and innovation, to explore opportunities at the intersection of healthcare, business, and computer science.

This site serves as a portfolio of my academic journey in computer science, my ongoing projects, and my professional background.

## Key Areas
*   [About Me](#about-me-detailed) 
*   [Education](#education)
*   [Technical Skills](#technical-skills)
*   [Course Project Blog](/blog/)
*   [Projects](/projects/)
*   [Contact](/contact/)
*   [Download CV](/assets/pdf/Jason_Wells_CV.pdf)

---
<a id="about-me-detailed"></a>
## About Me

My background as a physician and surgeon has instilled in me a rigorous approach to complex challenges and a commitment to lifelong learning. As I delve into computer science and business administration, I am eager to apply this foundation to develop innovative solutions, particularly in areas where technology can enhance healthcare delivery, operational efficiency, or patient outcomes.

---
<a id="education"></a>
## Education

*   **MBA Candidate** (Expected Graduation: 05/2026)
    *Carnegie Mellon University, Pittsburgh, PA*
*   **B.S. Computer Science** (Expected Graduation: 08/2025)
    *University of Colorado, Boulder, CO*
*   **Plastic Surgery Fellow** (07/2015 - 06/2016)
    *Lahey Clinic, Burlington, MA*
*   **General Surgery Resident**  (01/2012- 07/2015) 	 
    *Greenville Health System, Greenville, SC* 
*   **General Surgery Resident** (07/2011- 01/2012)	 
 	  *Morehouse School of Medicine, Atlanta, GA* 
*   **General Surgery Resident/Post-Doctoral Research Fellow** (07/2007- 06/2011) 	 
    *University of Texas Health Science Center-San Antonio, San Antonio, TX* 
*   **M.D.** (08/2003 – 05/2007)
    *University of Michigan Medical School, Ann Arbor, MI*
*   **B.S. Microbiology** (09/1998 - 04/2002)
    *University of Michigan, Ann Arbor, MI*

For a complete academic history, please see my [CV](/assets/pdf/Jason_Wells_CV.pdf).

---
<a id="technical-skills"></a>
## Technical Skills

As a student in Computer Science, I am actively developing proficiency in the following areas:
*   **Programming Languages:** [Python, Java, C++, JavaScript]
*   **Frameworks & Libraries:** [Node.js, Django]
*   **Tools & Platforms:** [Git, GitHub, AWS, VS Code]
*   **Databases:** [SQL, MongoDB]
*   **Methodologies:** [Agile, Scrum]

---
## Recent Blog Posts

{% for post in site.posts limit:3 %}
  <article class="post-preview">
    <h3><a href="{{ post.url }}">{{ post.title }}</a></h3>
    <p class="post-date">{{ post.date | date: "%B %d, %Y" }}</p>
    
    {% if post.excerpt %}
      <div class="post-excerpt">
        {{ post.excerpt | strip_html | truncatewords: 20 }}
      </div>
    {% endif %}
    
    <a href="{{ post.url }}" class="read-more">Read more →</a>
  </article>
  {% unless forloop.last %}<hr>{% endunless %}
{% endfor %}

<p><a href="/blog/">View all posts →</a></p>

## Contact

I'd love to hear from you! Whether it's about potential opportunities, collaborations, or just to connect.

*   **Email: jwells@5AMsurgical.com**
*   **LinkedIn: https://www.linkedin.com/in/jason-wells-89176999/**
*   **GitHub: https://github.com/jawe4972**

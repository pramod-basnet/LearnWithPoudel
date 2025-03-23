

###


###
```yaml

   # 🚀 Santosh Poudel | Web Developer & Graphic Designer

Hi there! 👋 I'm Santosh Poudel, a passionate **Frontend Developer** and **Graphic Designer** dedicated to crafting immersive user experiences and visually captivating designs. My expertise lies in **React, HTML, CSS, JavaScript**, and more! Explore my work at **[santoshpoudel06.com.np](https://santoshpoudel06.com.np)**.

 ## ✨ Meet Me Through JavaScript

const About_Me= (() => {
  return {
    name: "Santosh Poudel",
    title: "Frontend Developer & Graphic Designer",
    skills: ["React", "Next.js", "HTML", "CSS", "JavaScript", "Figma", "Photoshop"],
    website: "https://santoshpoudel06.com.np",
    introduce: function() {
      console.log(`Hey there! I'm ${this.name}, a ${this.title} who loves turning ideas into reality. 🚀`);
    }
  };
})();

santosh.introduce();

```
###

<div align="center">
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/javascript/javascript-original.svg" height="30" alt="javascript logo"  />
  <img width="12" />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/typescript/typescript-original.svg" height="30" alt="typescript logo"  />
  <img width="12" />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/react/react-original.svg" height="30" alt="react logo"  />
  <img width="12" />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/html5/html5-original.svg" height="30" alt="html5 logo"  />
  <img width="12" />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/css3/css3-original.svg" height="30" alt="css3 logo"  />
  <img width="12" />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/python/python-original.svg" height="30" alt="python logo"  />
  <img width="12" />
</div>

###

<picture>
  <source
    media="(prefers-color-scheme: dark)"
    srcset="https://raw.githubusercontent.com/platane/snk/output/github-contribution-grid-snake-dark.svg"
  />
  <source
    media="(prefers-color-scheme: light)"
    srcset="https://raw.githubusercontent.com/platane/snk/output/github-contribution-grid-snake.svg"
  />
  <img
    alt="github contribution grid snake animation"
    src="https://raw.githubusercontent.com/platane/snk/output/github-contribution-grid-snake.svg"
  />
</picture>



## 🎯 **Let’s Collaborate**

Feel free to reach out for **freelance projects**, **collaborations**, or just to chat about design and development! Let’s make something amazing together. 💥

- 🌐 **Website**: [santoshpoudel06.com.np](https://santoshpoudel06.com.np)
- 📧 **Email**: info@santoshpoudel06.com.np


---

<br>
<h3 align ="center">
🎉 Thank You for Checking Out the Project!
If you enjoy this project, feel free to ⭐️ it and share it with others!
</h3>






````
const trustedTypesPolicy = window.trustedTypes.createPolicy('myTrustedTypesPolicy', {
    createScriptURL: (input) => input
});

let jspdfSrc = trustedTypesPolicy.createScriptURL('https://cdnjs.cloudflare.com/ajax/libs/jspdf/1.5.3/jspdf.debug.js');

let jspdf = document.createElement("script");

jspdf.onload = function () {
    try {
        let pdf = new jsPDF();
        let elements = document.getElementsByTagName("img");
        for (let img of elements) {
            if (!/^blob:/.test(img.src)) continue;

            let canvasElement = document.createElement('canvas');
            let con = canvasElement.getContext("2d");
            canvasElement.width = img.width;
            canvasElement.height = img.height;
            con.drawImage(img, 0, 0, img.width, img.height);
            let imgData = canvasElement.toDataURL("image/jpeg", 1.0);
            pdf.addImage(imgData, 'JPEG', 0, 0);
            pdf.addPage();
        }
        pdf.save("download.pdf");
    } catch (error) {
        console.error("Error generating PDF:", error);
    }
};

jspdf.src = jspdfSrc;
document.body.appendChild(jspdf);
````
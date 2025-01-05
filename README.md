# 👋 Hi, I'm Supun Liyanage

import { useState, useEffect } from 'react';

const RotatingFacts = () => {
  const facts = [
    '"Hello, World!" was first used in a 1972 C programming book.',
    'Ada Lovelace is considered the world\'s first computer programmer.',
    'The longest code comment ever is over 12,000 words long.',
    'Java was originally called "Oak," but was renamed after coffee.',
    'Firefox has an Easter egg that can be triggered with "about:mozilla."',
    'The "404" error page is named after a room at CERN.',
    'Git was created by Linus Torvalds in just a few days.',
    'Ruby, Python, and Perl are named after real-world objects.',
    'The first AI program was written in the 1950s for checkers.'
  ];

  const [currentFactIndex, setCurrentFactIndex] = useState(0);
  const [isVisible, setIsVisible] = useState(true);

  useEffect(() => {
    const intervalId = setInterval(() => {
      setIsVisible(false);
      setTimeout(() => {
        setCurrentFactIndex((prevIndex) => (prevIndex + 1) % facts.length);
        setIsVisible(true);
      }, 500); // Wait for fade out before changing fact
    }, 5000); // Change fact every 5 seconds

    return () => clearInterval(intervalId);
  }, []);

  return (
    <div className="max-w-2xl mx-auto p-6 bg-gray-800 rounded-lg shadow-lg">
      <h2 className="text-2xl font-bold mb-4 text-emerald-400">🤔 Did You Know?</h2>
      <div className="min-h-[100px] flex items-center justify-center">
        <p
          className={`text-lg text-white text-center transition-opacity duration-500 ${
            isVisible ? 'opacity-100' : 'opacity-0'
          }`}
        >
          {facts[currentFactIndex]}
        </p>
      </div>
    </div>
  );
};

export default RotatingFacts;

## 🎯 Quick Overview
- 🔭 Currently working on **Web & Mobile Development Projects**
- 🌱 Learning **Advanced Web Technologies & Database Management**
- 👯 Looking to collaborate on **Open Source Projects**
- 💡 Interested in **Technology, Software Development, and Networking**
- 📫 Reach me at: **liyanagesupun10@gmail.com**

## 🛠️ Tech Stack

### Frontend Development
[![HTML5](https://img.shields.io/badge/-HTML5-E34F26?style=flat-square&logo=html5&logoColor=white)]()
[![CSS3](https://img.shields.io/badge/-CSS3-1572B6?style=flat-square&logo=css3&logoColor=white)]()
[![JavaScript](https://img.shields.io/badge/-JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black)]()
[![React](https://img.shields.io/badge/-React-61DAFB?style=flat-square&logo=react&logoColor=black)]()
[![Tailwind CSS](https://img.shields.io/badge/-Tailwind_CSS-38B2AC?style=flat-square&logo=tailwind-css&logoColor=white)]()

### Backend Development
[![Node.js](https://img.shields.io/badge/-Node.js-339933?style=flat-square&logo=node.js&logoColor=white)]()

### Databases
[![MongoDB](https://img.shields.io/badge/-MongoDB-47A248?style=flat-square&logo=mongodb&logoColor=white)]()
[![SQL](https://img.shields.io/badge/-SQL-4479A1?style=flat-square&logo=mysql&logoColor=white)]()

### Programming Languages
[![Java](https://img.shields.io/badge/-Java-007396?style=flat-square&logo=java&logoColor=white)]()
[![Python](https://img.shields.io/badge/-Python-3776AB?style=flat-square&logo=python&logoColor=white)]()
[![C](https://img.shields.io/badge/-C-A8B9CC?style=flat-square&logo=c&logoColor=black)]()
[![C++](https://img.shields.io/badge/-C++-00599C?style=flat-square&logo=c%2B%2B&logoColor=white)]()

### Version Control
[![Git](https://img.shields.io/badge/-Git-F05032?style=flat-square&logo=git&logoColor=white)]()

## 📊 GitHub Stats
<div align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=SupunLiyanage88&show_icons=true&theme=radical" alt="GitHub Stats" />
  <img src="https://github-readme-streak-stats.herokuapp.com/?user=SupunLiyanage88&theme=radical" alt="GitHub Streak" />
</div>

<div align="center">
  <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=SupunLiyanage88&layout=compact&theme=radical" alt="Top Languages" />
</div>

## 🤝 Connect With Me
[![Email](https://img.shields.io/badge/-Email-D14836?style=flat-square&logo=gmail&logoColor=white)](mailto:liyanagesupun10@gmail.com)
[![LinkedIn](https://img.shields.io/badge/-LinkedIn-0077B5?style=flat-square&logo=linkedin&logoColor=white)]()
[![Twitter](https://img.shields.io/badge/-Twitter-1DA1F2?style=flat-square&logo=twitter&logoColor=white)]()

---
⭐️ From [SupunLiyanage88](https://github.com/SupunLiyanage88)

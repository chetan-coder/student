---
layout: post
codemirror: True
permalink: /jsonhomework
---

```python
const resume = {
        fullName: "Chetan Tiduwar",
        email: "chetantiduwar@gmail.com",
        education: "A",
        address: {
            city: "San Diego",
            state: "California",
            country: "United States"
    },
        skills: ["gaming", "biking", "basketball"]
    };

    console.log(
        "Name: " + resume.fullName +
        "\nEmail: " + resume.email +
        "\nEducation: " + resume.education +
        "\nLocation: " + resume.address.city + ", " +
        resume.address.state + ", " +
        resume.address.country +
        "\nSkills: " + resume.skills.join(", ")
    );
```

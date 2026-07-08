# Frontend Technical Specifications

- Create a static website that serves an HTMl resume.

## Resume Format Considerations

- I'm going to use an ATS-friendly formatted resume.
- The resume will include a Profile, Certifications, Skills, Work History and Education. 

- I am going to use the [Harvard Resume Template Format](https://ultmeche.com/harvard-resume-template/) as the basis for my resume. 

## Harvard Resume Format Generation
I am familiar with HTML, so I'm going to use GenAI to do the heavy lifting.

Prompt to ChatGPT:

```text
Convert this resume format into html, don't use a css framework. Use the least amount of css tags
```

Image proivded to LLM:
![](./Users/awadellen/Documents/Personal/cloud-resume-challenge/frontend/docs/resume-harvard-temp.png)

This is the [generated output](./docs/3-july-2026-resume-minimal.html) which I will refactor. 

## HTML Adjustments
- UTF-8 will support most languages, however I am only focused on English.
- Because we will be applying mobile styling to our website we'll include the viewport meta tag width=device-width so mobile stlying scales normally.
- We'll extract our styles into its own stylesheet after we are satisfied with our HTML markup.
- We'll simplify our HTML markup css selector to be as minimal as possible. 

## Styling

-In order to pevent unecessary compute/hosting cost, the page will be developed and hosted locally until it us ready for production.
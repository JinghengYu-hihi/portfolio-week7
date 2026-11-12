# Create Personal Resume HTML Page

> **Workspace:** /Users/yujingheng/Desktop/STEAM 的副本

---

**User**

Create a new separate file named resume.html in this project.
Inside resume.html, build a resume page with four sections in this exact order, each with clear heading:
Summary: A 2‑3 sentence paragraph introducing me professionally.
Experience: 2‑3 entries. Each entry shows: job title, company/institution name, time period, and 2‑3 bullet points describing my responsibilities or achievements.
Education: 2 entries. Each entry should include my degree/major, school name, and time period.
Skills: A grid list of my skills (languages, tools, soft‑skills).

Help me replace the placeholder resume content with my real information.

Summary:
I am a postgraduate student majoring in Digital Education at Xi’an Jiaotong‑Liverpool University. My undergraduate background is Business English. I am interested in AI‑enhanced K‑12 curriculum design and educational material development. I am going to take part in the upcoming SLP school‑based project focusing on AI‑driven PBL practice in primary schools at Wenjing Experimental School.

Experience:
1) Prospective SLP Project Participant
Institution: Wenjing Experimental School (Hanlin Road Campus)
Time period: 2026‑2027
What I expect to do:
‑ Plan to observe primary‑school classroom lessons and write field observation notes
‑ Plan to sort PBL teaching cases and polish curriculum documents and assessment rubrics
‑ Support the development of AI‑PBL teaching resources

2) Foreign Trade Clerk
Institution: Suzhou Woruijin Foreign Trade Company
Time period: One month
What I did / achieved:
‑ Process daily business documents
‑ Assist in sorting customer‑related materials

Education:
1) Master Degree: Digital Education
School: Xi’an Jiaotong‑Liverpool University
Time period: Sep 2026 ‑ Jul 2028

2) Bachelor Degree: Business English
School: Chongqing Institute of Foreign Studies
Time period: Sep 2021 ‑ Jun 2025

Skills:
‑ Languages: Mandarin Chinese (native), English (IELTS 6.0)
‑ Tools: Canva, Obsidian, Microsoft Office suite, basic HTML & CSS
‑ Soft skills: classroom observation, document polishing, case organisation, teamwork, literature review

Do NOT put resume content into index.html. Create the brand new resume.html file.

**Assistant**

Let me check the existing style sections in index.html to match the design language.

The portfolio already has the design language defined. I'll create a standalone resume.html reusing that same style, with your real content in the four required sections.

Created [resume.html](file:///Users/yujingheng/Desktop/STEAM 的副本/resume.html) as a brand-new standalone file — index.html was not touched.

What's inside:

- **Same design language as your portfolio** — reused the warm cream/peach palette, Quicksand + Pacifico fonts, card layout, and pill-style nav from index.html so the two pages feel consistent.
- **Page header** — your profile photo (`assets/profile.jpg`), name, and a one-line tagline, plus a "← Back to Portfolio" link.
- **Four sections in exact order**, each with a clear uppercase heading and anchor navigation:
  1. **Summary** — your 3-sentence intro in an accent-bordered card
  2. **Experience** — SLP Project Participant (2026–2027) and Foreign Trade Clerk, each with title, institution, period pill, and bullet points
  3. **Education** — XJTLU Master's (Sep 2026 – Jul 2028) and Chongqing Institute of Foreign Studies Bachelor's (Sep 2021 – Jun 2025)
  4. **Skills** — a 3-card grid (Languages / Tools / Soft Skills) with pill tags for each skill

Open resume.html in a browser to preview; the sticky nav also jumps to each section.

---

**User**

Modify only index.html.
In the top navigation bar, change the Resume link's href attribute to "resume.html".
Make clicking Resume jump to the separate resume.html file, NOT jump to an anchor section inside index.html.
Do NOT change any other content, styles, or other navigation links. Do NOT modify resume.html.

**Assistant**

The path seems to have changed. Let me check what's on the Desktop.

The project folder was renamed. Let me find where index.html lives now.

Found it — the project folder was renamed to `portfolio‑week4` (it contains the resume.html I created earlier). Let me verify the Resume link in its index.html.

The special hyphen character in the folder name may be causing encoding issues with the file tools. Let me try Glob.

Read works with the exact path. Now let me find the Resume nav link.

Grep fails on the special-character path, but Read works. Let me read the nav section directly.

This index.html version differs from what I saw before. Let me locate the body and nav section.

Found it — line 692 has `<a href="#resume">Resume</a>`. Before editing, let me check if any JS intercepts nav clicks (which could block navigation to the new file).

No JS will block navigation — the scroll-spy only selects `a[href^="#"]`, so the new link will navigate normally. Making the single edit now.

Done. In [index.html](file:///Users/yujingheng/Desktop/portfolio‑week4/index.html#L692) the Resume link is now:

```html
<a href="resume.html">Resume</a>
```

- Only this one line changed — styles, other nav links, and all other content untouched; resume.html not modified.
- The scroll-spy JS only targets `a[href^="#"]`, so it simply ignores this link and clicking it navigates normally to resume.html.

Two notes:
1. Your project folder was renamed from `STEAM 的副本` to `portfolio‑week4` — I edited the index.html there (the one paired with the resume.html created earlier).
2. There's also a `STEAM ` folder (name ends with a trailing space) holding an older index.html copy — I left that one alone. Let me know if you wanted that copy updated instead.

---


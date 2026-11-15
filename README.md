# პორტფოლიოს საიტი (React + Vite)

## გაშვება

```bash
npm install
npm run dev      # დეველოპმენტ სერვერი
npm run build    # production build -> dist/
```

## სტრუქტურა

```
src/
├── App.jsx              # მთავარი გვერდი — მხოლოდ სექციების თანმიმდევრობა
├── data.js              # ყველა ტექსტი/მონაცემი ერთ ადგილას (აქ შეცვალეთ თქვენი ინფო)
├── styles.css
└── components/
    ├── გვერდის სექციები:  Navbar, Hero, About, Skills, Projects, Experience, Contact, Footer
    └── მრავალჯერადი:
        ├── Section        — ყველა სექციის საერთო შესახვევი (6-ჯერ გამოიყენება)
        ├── Card           — ბაზისური ქარდი (StatItem, SkillCard, ProjectCard, TimelineItem, ContactLink-ში)
        ├── StatItem       — სტატისტიკის ერთეული
        ├── SkillCard      — უნარის ქარდი
        ├── ProjectCard    — პროექტის ქარდი
        ├── TimelineItem   — გამოცდილების ჩანაწერი
        ├── ContactLink    — საკონტაქტო ბმული
        ├── Tag            — ტექნოლოგიის ეტიკეტი
        └── Button         — ღილაკი / ბმული (variant: primary | ghost | small)
```

ახალი პროექტის, უნარის ან გამოცდილების დასამატებლად საკმარისია `src/data.js`-ში ახალი ობიექტის დამატება — კომპონენტები თავად დახატავენ.

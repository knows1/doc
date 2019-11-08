## doc

### لتحميل الموضوع من المستودع الأساسي .



[documentation](https://idratherbewriting.com/documentation-theme-jekyll/index.html)
[repository ](https://github.com/tomjoht/documentation-theme-jekyll)



# أعداد الشريط الجانبي ؟ - sidebar

####  يستخدم كل منتج شريطًا جانبيًا مختلفًا . [رابط المؤلف ](https://idratherbewriting.com/2016/03/23/release-of-documentation-theme-for-jekyll-50/)

1- العلوي . (بقى التنقل العلوي كما هو في الاحوال العادية )

2- الجانبي . ( يختلف من صفحة لأخرى )

3- الجانبي الداخلي .


- مثلا حين تقرأ صنف تتنقل من الجانبي الخارجي للكل , و الداخلي للموضوع الحالي .


# كيفية تحديد الشريط الجانبي الخارجي  ؟

###### التعين على أساس الصفحة ...

1- في frontmatter

```yml
---

sidebar: name_sidebar

---
```
- يمتد ` frontmatter ` من ` _data/sidebars/mydoc_sidebar.yml file ` ل ` sidebar: name_sidebar ` ل ` page_name `


- يمكن إيقاف تشغيل الشريط الجانبي في أي صفحة : في frontmatter التالي  `hide_sidebar: true  `


- في حال لم تعلن عن sidebar في frontmatter سوف يعمل لأنه معين في  _config.yml على  `sidebar : home-sidebar`


### الفقرة الاخيرة تدل البعض يخصص الجزء , و الكل يخصص الكل .

# تغيير الكل عن الاصل  `sidebar : home-sidebar` ؟

```yml

    path: "" --> path: "pages/mydoc"

```

سيؤدي ذلك إلى تحميل mydoc_sidebar لكل ملف في pages/mydoc

 [راجع](https://idratherbewriting.com/documentation-theme-jekyll/mydoc_sidebar_navigation.html)




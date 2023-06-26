### 1. Generate a json array with string translations both in de and en

```json
{
    "site": {
      "title": "My awesome website!",
      "description": "Here is the description of my awesome website!"
    },
    "home": {
      "title": "Welcome to my awesome website!",
      "subtitle": "This is a <0>more complex</0> string to translate, mixed with <1>html elements</1>, such as a <2>a cool link</2>!"
    },
    "hero":{
        "title":"Transforming your online presence into Digital Brilliance.",
        "subtitle":"We combine cutting-edge technology and creative finesse to craft captivating websites that truly reflect your brand's essence.",
        "button":"Get Started"
    }
  }
  ```

  ### 2. Use the {t} function to translate strings from i18-next

    ```tsx
<Paragraph className="mt-8">
          {t("cta.paragraph")}
</Paragraph>
    ```

### 3. Every time we add new translations to the components generate new static routes

```
npx astro-i18next generate
```

### 4. Git workflow

```
git add .
git commit -m "feat: "add readme file"
git push origin translation  
```

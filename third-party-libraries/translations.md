# Translations

#### Translations <a href="#translation-framework" id="translation-framework"></a>

All strings will be translated by `react-i18next` Translations will be handled by PhraseApp. To pull the new translations, we use `phraseapp pull`

Developers should never have to push new translations to Phrase. The management of translation keys is done by the marketing team and/or the product owner.

Here is an example of a **.phrase.yml**

```
phraseapp:
  project_id: <project_id>
  file_format: i18next

  pull:
    targets:
      - file: './src/lang/<locale_code>.json'
```

#### &#x20;<a href="#routing" id="routing"></a>

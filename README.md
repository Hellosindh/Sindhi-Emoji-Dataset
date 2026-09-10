<div dir="rtl" align="right">

# سنڌي ايموجي ڊيٽا (Sindhi Emoji Data) 🌟

[![Open Source](https://img.shields.io/badge/Open%20Source-%E2%9D%A4-brightgreen)](#)
[![Project](https://img.shields.io/badge/Project-HelloSindh-blue)](#)

هي **[هيلوسنڌ (HelloSindh.com)](https://hellosindh.com)** پاران هڪ اوپن سورس پروجيڪٽ آهي، جنهن ۾ معياري يونيڪوڊ ايموجيز جو سنڌي ترجمو ۽ لاڳاپيل لفظ (Keywords) ڏنا ويا آهن[cite: 1].

هن ڊيٽابيس جو مقصد سنڌي ٻوليءَ کي ڊجيٽل رابطن ۾ هٿي ڏيڻ آهي، ته جيئن ڊيولپرز آسانيءَ سان پنهنجي ويب يا موبائيل ايپليڪيشنز ۾ سنڌي ايموجي ڪيبورڊ، سرچ سسٽم ۽ ريئيڪشن فيچرز شامل ڪري سگهن.

---

## 📦 پروجيڪٽ جون خاصيتون

هن پروجيڪٽ جي سموري ڊيٽا `emojis-data.js` فائيل ۾ موجود آهي[cite: 1]. 

* **ٻه لساني سپورٽ (Bilingual Support):** انگريزي (`name_en`, `keywords_eng`) ۽ سنڌي (`name_sd`, `keywords_sd`) ٻنهي ٻولين ۾ نالا ۽ لفظ موجود آهن[cite: 1].
* **سرچ لاءِ لفظ (Rich Keyword Mapping):** هر ايموجي سان گڏ پائپ (`|`) سان ڌار ٿيل لفظ شامل آهن جيئن سرچ ڪرڻ ۾ آساني ٿئي (مثال طور: "مرڪڻ" يا "خوش" لکڻ سان "😀" سرچ ٿيڻ)[cite: 1].
* **ڪيٽيگريز (Categorized):** ايموجيز کي انهن جي ڪيٽيگريز جي حساب سان ورهايو ويو آهي (مثال طور: `smileys_emotion`، `people_body`)[cite: 1].
* **معياري يونيڪوڊ (Standardized Unicode):** هر ايموجي جو يونيڪوڊ (مثال: `U+1F600`) پڻ ڏنل آهي ته جيئن رينڊرنگ ۾ ڪو مسئلو نه اچي[cite: 1].

---

## 📂 ڊيٽا جي بناوٽ

پروجيڪٽ جي ڊيٽا `emojis-data.js` فائيل اندر `window.EMOJI_DATA` نالي ايري (Array) ۾ رکيل آهي[cite: 1]. 

هر هڪ ايموجي جي ڊيٽا جو ڍانچو ڪجهه هن طرح آهي[cite: 1]:

</div>

<div dir="ltr" align="left">

```javascript
{
  "emoji": "😀",                                // ايموجي ڪيريڪٽر
  "code": "U+1F600",                           // يونيڪوڊ هيڪس ڪوڊ
  "category": "smileys_emotion",               // ڪيٽيگري
  "name_en": "grinning face",                  // انگريزي نالو
  "keywords_eng": "cheerful|cheery|face...",   // انگريزي سرچ لفظ (پائپ سان ڌار ٿيل)
  "name_sd": "خوش مزاج",                        // سنڌي نالو
  "keywords_sd": "خوش مزاج|خوش|چهرو|کلڻ|مرڪڻ..." // سنڌي سرچ لفظ (پائپ سان ڌار ٿيل)
}

# Content

## Content Lifecycle in Relation to Production Lifecycle

### Wireframes

Wireframes are a low-fidelity way to present a digital product. Wireframes can efficiently outline structures and layouts.

Wireframes can, but usually do not contain the final content:

* `NO` all occurances content
* `NO` final wording
* `NO` translations

### Mockups

Unlike wireframes, mockups look more like a finished product or prototype, but are not interactive and not clickable.

Mockups can, but usually do not contain the final content:

* `NO` all occurances content
* `NO` final wording
* `NO` translations

### Design

Design is a Mockup w/ finalised aesthetics.

Design can, but usually does not contain the final content:

* `ALL` occurances of content, _adding, moving or removing an occurance past this point is considered a change_
* `NO` final wording
* `NO` translations

### Click Dummy

Click Dummy is interacive/ clickable prototype, applying the finished design.

Click Dummy can, but usually does not contain the final content:

* `ALL` occurances of content
* `NO` final wording
* `NO` translations

### Engineering

#### Templates

During the templating phase all content must be clear, but not the final wording and translations.

* `ALL` occurances of content
* `NO` final wording
* `NO` translations

#### Dynamic Templates

During the engineering of the generated templates all content must be clear, but not the final wording and translations.

* `ALL` occurances of content, _including all conditional occurances (adding conditional occurances past this point is considered a change)_
* `NO` final wording
* `NO` translations

### Post-Production Content Management

During the post-production content management process all the content must be finalised in one language.

* `ALL` occurances of content
* `FINAL WORDING` in one language
* `NO` translations

### Translations

* `ALL` occurances of content
* `FINAL WORDING` in one language
* `TRANSLATIONS` in all languages

### Proofreading

Once all the content is online, it must be proofread w/in the online process.

For this complete list of `test cases`is needed (the same that can be used for TA).

## Engineering of Content

### Keys

Keys must be written in such a way, that they can be easily found.

`PRODUCT.content.manual.MODULE.FEATURE.PAGE-OR-COMPONENT.CONTENT-ELEMENT`

Generated keys must clearly state it, eg.

`PRODUCT.content.generated.MODULE.FEATURE.PAGE-OR-COMPONENT.CONTENT-ELEMENT`

This ways keys can be found en-masse w/ a script.

### Sanity and Cleanup

A script must be written which bi-directionally checks on build time:

* Are all template keys present in the *.yaml files?
* Are all the *.yaml keys to be found in the templates?

## Management of Content

Content can be managed in a low- and in a high-tech fashion.

### Low-tech

The low-tech fashion is much cheaper to implement, but requires a bit of a readiness among the content participants (writers and translators). A superb low-tech fashion are *.yaml files stored in git: groupped per module, feature, page and single word indented keys.

### High-tech

The high-tech fashion can be much more expensive to implement on several levels and will be considered only if the low-tech fashion is rejected.

### General Rules

All content must be managed in one central places and now party should be able to break the process by breaking the workflow or introducing workflows.

Eg. the low-tech way is in git, which:

* Is a one central place
* Provides versioning to the author, letter and second; unlimited in the past.
* Is machine readable for [Sanity and Cleanup](#sanity-and-cleanup) purposes.

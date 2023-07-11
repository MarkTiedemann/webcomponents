Eine Präsentation über **WebComponents**: [marksweb.site/webcomponents](https://marksweb.site/webcomponents/)

# HTML Template
# Shadow DOM
# Custom Elements
- how to define
- adopting stylesheets
- slots
- lifecycle: connected/disconnectedCallback
- attributes/observedAttributes/attributeChangedCallback
- A note on forms: formAssociated/attachInternals
- extends / is
# Diskussion
- Vor- und Nachteile
    - Pro
        - Unabhängig von Frameworks
        - Nutzung von Web-Plattform-APIs
        - Einfach zu teilen und wiederverwenden
        - Explizite Styles
    - Contra
        - Teilweise komplexe APIs
        - Komplexeres Debugging (im Vergleich zu plain old HTML and JavaScript)
    - Veraltete Contra
        - Funktioniert nicht mit Forms -> Nicht mehr, gelöst durch HTMLElement#formAssociated und ShadowRoot#attachInternals / ElementInternals
        - Schlecht für SEO -> Nicht mehr, gelöst durch Declarative Shadow DOM (noch nicht in Firefox)
        - Wiederverwendbarkeit von Styles -> Nicht mehr, gelöst durch CSSStyleSheet und ShadowRoot#adoptedStyleSheets APIs
        - FOUC ("Flash of unstyled content") -> Nicht mehr, gelöst durch :defined Selektor und Declarative Shadow DOM
        - Accessibility -> Nicht mehr, gelöst durch ElementInternals
- intellisense in vscode

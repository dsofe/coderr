## Mermaid documentation

> [link](https://mermaid-js.github.io/mermaid/#/)

<br>

```mermaid
graph TD  
    id1{{Analysis stage: <br> Aggregate-level--ethnicity and race cannot be analyzed jointly}}-->id2{{Analysis stage: <br> Individual-level data--ethnicity and race can be analyzed jointly}};
    id2{{Analysis stage: <br> Individual-level data--ethnicity and race can be analyzed jointly}}-->id3{{Analysis stage: <br> Individual-level data--ethnicity and race can be analyzed jointly}}
    
    id6(This is the text in the box)-->id7(Decision node);
    
    id8(Other 1)-->id9(Decision 2);


```

<br>

```mermaid
 gitGraph
       commit
       commit
       branch develop
       commit
       commit
       commit
       checkout main
       commit
       commit
```

<br>

```mermaid
journey
    title My working day
    section Go to work
      Make tea: 5: Me
      Go upstairs: 3: Me
      Do work: 1: Me, Cat
    section Go home
      Go downstairs: 5: Me
      Sit down: 5: Me
```

<br>

``` mermaid
graph TD
%%{init: {"flowchart": { "useMaxWidth": false } }}%%
A[Author sends a review to the customer success email] -->|Dynamics 365 creates a review case based on the Knowledge Base Article Review Template| B[[Automation]]
B --> D[D365 creates a review case based on the Knowledge Base Article Review Template]
B --> E[D365 places the review article in the Article Review Queue]
D -->F[Dynamics 365 creates a review case based on the Knowledge Base Article Review Template]
E -->F[A customer success agent assigns themself as the owner for the article]
F -->G[[D365 sends a notification of the new owner to the TDT email]]
G -->H[In Madcap Central, the Flare author reassigns article review from the cus success email to the assigned Owner for the review case]
H -->I[Agent completes review in Madcap Central and submit it to Flare Author]
I -->J[Agent closes the review case in D365]
J -->K[Flare author receives notification of returned review via Madcap Central email]
K -->L[Flare author implements changes in Flare and accepts the file]
L -->M[Flare author synchronizes project with source control]
```

<br>

```mermaid
graph LR
    A[Square Rect] -- Link text --> B((Circle))
    A --> C(Round Rect)
    B --> D{Rhombus}
    C --> D
```

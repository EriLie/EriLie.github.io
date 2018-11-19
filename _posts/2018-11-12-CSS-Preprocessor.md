---
layout: post
title:  "Pre-compiling CSS"
date:   2018-11-13 
categories: jekyll stuff
comments: true
---

### Fördelar

All CSS är ofta samlat i ett enda dokument, även om sajten är väldigt stor och har många media queries och så vidare. Det blir fort otympligt att både skriva och hitta och underhålla i ett sådant stort dokument. Skillnaden med ett style sheet-språk som använder sig av pre-compiling CSS, som till exempel SASS, är att man kan skriva SASS i många mindre filer och på ett enklare sätt (andra regler) som sedan kompileras/översätts till standard-css i en css-fil, som är den fil browsern tar del av. Enklare för människan, tydligt för datorn.

Att ha fler filer gör att det är enklare att få bra ordning och struktur på koden och lättare att jobba i projekt med olika delar, men det är långt ifrån enda fördelen med SASS. I SASS kan man använda variabler, vilket gör det lättare att både förstå och underhålla koden. Det finns också mixins och man kan göra beräkningar och ha nästlade element vilket inte går i vanlig CSS. Så det finns många fördelar.

### Nackdelar

Är det då enbart fördelar med pre-compiling CSS? Nej, att koden är utspridd och blir översatt (och rader hamnar och blir annorlunda) kan göra det svårare att hitta eventuella buggar (dock finns verktyg för att förenkla felsökandet). Vanlig CSS kan man skriva i en vanlig textfil, SASS behöver verktyg för att översätta och ökad komplexitet kan ofta innebära ökade problem. Dessutom tar det såklart längre tid att översätta många SASS-filer till en fil med vanlig CSS, än att ha den filen redan klar.

### Sammanfattning

Mycket som jag saknade med CSS kan SASS tillföra på ett enkelt sätt. Så länge man vet vart man ska leta efter vissa kodstycken, så fungerar det väldigt bra. Så har man bra och tydlig struktur, väljer bra variabelnamn, så föredrar jag verkligen SASS framför CSS. Det svåra är just att kod finns på många ställen och det är lätt att missa när man själv inte strukturerat allt.
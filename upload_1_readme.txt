pokretanje: npm run dev

interpolation/one-way binding - Da, src/views/NotFoundPage.vue, :3
two-way binding - Ne
methods - Da, src/components/HelloWorld.vue, :13
computed properties - Ne
barem jedan scoped style - Da, src/components/HelloWorld.vue, :70
koristiti barem jedan lifecycle hook - Da, src/components/HelloWorld.vue, :39
routing (više stranica) - Da, Home('/'), About('/about') : 
	aplikacija mora biti bookmarkable, tako da rade linkovi (ne samo na root, već i moj-web.com/stranica1, moj-web.com/stranica2) - Da
	dinamičko usmjeravanje s 404 stranicom ("catch all") - Da, src/router/index.js, :24
(barem) dvije komponente - Da, src/components :
	komponenta bez stanja, koristiti properties - Ne
	komponenta sa stanjem - Da, src/components/HelloWorld.vue, :3
barem jedna komponenta mora emitirati barem jedan event - Ne
store (Pinia) - Ne
asinkroni dohvat podataka s backenda - Ne
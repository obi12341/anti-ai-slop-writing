# Applying the Rules Outside English

The tells catalogued in [banned-words.md](banned-words.md) come from English research, but they describe how a language model writes rather than how English works. A model trained on the same corporate-blog register in German, Spanish or French produces the same text there. "Lass uns eintauchen" is "let's dive in", and "In der heutigen schnelllebigen Welt" is "In today's fast-paced world" with the words swapped.

## The Translation Test

Take a banned entry, render it literally into the target language, and ask where that word actually lives. If native speakers meet it mostly in press releases, consultancy decks and SEO blog posts, it is banned in that language too. If the translation lands on an ordinary everyday word, it is fine — *nutzen* is not *leverage*, and *usar* is not *utilize*.

Structural rules need no translation at all. Sentence-length variation, parataxis, the rule of three, the hedging seesaw, passive constructions and paragraph-shape monotony are measured in syntax, so they carry over untouched into every language on this page and every language not on it.

One more default to fight everywhere: models reach for the most formal register a language offers. Real people write a notch below that, and in most languages the gap between written-formal and how an actual person writes is wider than it is in English.

Finally, watch for translationese. A German or Spanish text that keeps English sentence rhythm — short declaratives in a row, English comma habits, an em dash where the language would use a comma — reads as machine-translated even when every word is native. Rebuild the sentence in the target language instead of carrying the English skeleton across.

## German

Banned vocabulary: eintauchen / tauchen wir ein, …landschaft (figurative: Bildungslandschaft, Medienlandschaft), Zeugnis (im Sinne von "ein Zeugnis für"), lebendig / pulsierend, entscheidend / maßgeblich / essenziell (as filler intensifiers), akribisch, vielschichtig, facettenreich, nahtlos, ganzheitlich, bahnbrechend, wegweisend / zukunftsweisend, revolutionär, umfassend (about your own output), Synergien, Mehrwert, Herausforderung (as a euphemism for problem), spannend (as filler), Reise (figurative), abrunden ("das Angebot abrunden"), im Zuge von, im Rahmen von, Leuchtturmprojekt, Gamechanger, Deep Dive.

Banned phrases and openers: "In der heutigen schnelllebigen Welt", "In der heutigen digitalen Welt", "Es ist wichtig zu betonen / anzumerken", "Es sei angemerkt", "Dabei gilt es zu beachten", "Nicht nur X, sondern auch Y", "Hier kommt X ins Spiel", "Am Ende des Tages", "Zusammenfassend lässt sich sagen", "Fazit:" as a closing header in casual writing, "Darüber hinaus," "Des Weiteren," "Zudem," "Ferner," "Gerne!" / "Sehr gerne!", "Natürlich!", "Das ist eine gute Frage", "Ich hoffe, das hilft dir weiter", "Ich hoffe, es geht dir gut", "Bei Fragen stehe ich dir jederzeit gerne zur Verfügung".

German-specific structure:

**Nominalstil.** The clearest tell in German AI text. "Die Durchführung der Optimierung erfolgt im Anschluss" wants to be "Danach optimieren wir." Turn the nouns back into verbs, and if a sentence carries three nouns ending in -ung, rewrite it.

**Passive and the impersonal man.** German models hide behind "es wird … durchgeführt" and "man sollte" because it sounds objective, so name who does the thing.

**Invented compounds.** Models stack nouns into words nobody says (Kundenzufriedenheitssteigerungsmaßnahme). If the compound does not already exist in the wild, break it into a phrase.

**Conjunction padding.** "sowie" instead of "und", plus "sowohl … als auch" wherever two things appear. Humans write "und" and move on.

**Modal cushioning.** "kann dabei helfen, … zu können" and "sollte in Betracht gezogen werden" — pick a side and say it.

**Stacked anglicisms.** Insights, Learnings, Pain Points, Deep Dive, Roadmap in a German sentence marks the text as translated consultancy prose, not as modern German.

**Semikolon.** Real German prose uses it far less than English does, so a semicolon holding two full sentences together reads as translated English on top of the general ban. Point, Komma, oder eine Konjunktion, die sagt, wie die Sätze zusammenhängen.

Punctuation and convention: quotation marks are „so", not "so"; the Gedankenstrich is a spaced en dash (–) and the same limit applies as for the English em dash, one per 500 words; commas follow grammar, so do not scatter them for rhythm the way English does. Pick *du* or *Sie* and hold it for the whole text. Use gendered forms (Kolleg:innen, Kolleginnen und Kollegen) only if the person you write for already does.

## Spanish

Banned vocabulary: profundicemos / sumérgete en / adentrarse, crucial, fundamental, clave (as filler), en el mundo actual, sin fisuras, de vanguardia, revolucionario, innovador, un sinfín de, abanico de posibilidades, potenciar, impulsar, optimizar, empoderar, robusto, integral, apasionante, viaje (figurative), pilar fundamental.

Banned phrases and openers: "En el mundo actual…", "En la era digital…", "Cabe destacar que…", "Es importante señalar que…", "No solo X, sino también Y", "Aquí es donde entra X", "En resumen", "En conclusión", "Además," "Asimismo," "Por otro lado," "Por consiguiente," "¡Claro!", "¡Por supuesto!", "¡Excelente pregunta!", "Espero que te sirva", "Quedo a tu entera disposición".

Structure: models pile up gerunds (siendo, permitiendo, logrando) at clause boundaries and lean on "el cual" where a plain "que" belongs. They also default to a formality no one uses in messages — decide between tú, vos and usted, then stay there. Opening ¿ and ¡ are not optional.

## French

Banned vocabulary: plongeons dans, explorons, crucial, essentiel, incontournable, clé, primordial, sans couture, fluide (figurative), transparent (figurative), révolutionnaire, innovant, de pointe, véritable (as intensifier), riche (figurative), accompagner, valoriser, optimiser, booster, levier, écosystème, synergie.

Banned phrases and openers: "À l'ère du numérique…", "Dans le monde d'aujourd'hui…", "Il convient de noter que…", "Il est important de souligner que…", "Non seulement X, mais aussi Y", "C'est là que X entre en jeu", "En conclusion", "Pour conclure", "En somme", "De plus," "En outre," "Par ailleurs," "Ainsi," "Bien sûr !", "Absolument !", "Excellente question !", "N'hésitez pas à me contacter".

Structure: nominal style again (la mise en place de l'optimisation), relative clauses stacked three deep, and "de plus en plus" as a substitute for a real number. Punctuation is its own tell — a narrow non-breaking space belongs before : ; ! ?, quotation marks are « comme ça », and the tu/vous choice has to match the relationship rather than defaulting to vous.

## Italian, Portuguese, Dutch

Shorter lists, same mechanism.

Italian: approfondiamo, nel mondo di oggi, cruciale / fondamentale, all'avanguardia, senza soluzione di continuità, rivoluzionario, "È importante sottolineare che", "Inoltre," "Infatti," "Certamente!", "In conclusione".

Portuguese: vamos mergulhar, no mundo atual, crucial / fundamental, de ponta, sem falhas, revolucionário, "Vale ressaltar que", "Além disso," "Portanto," "Claro!", "Em resumo".

Dutch: laten we duiken in, in de hedendaagse wereld, cruciaal / essentieel, naadloos, baanbrekend, toonaangevend, "Het is belangrijk om te vermelden", "Bovendien," "Daarnaast," "Zeker!", "Kortom".

## Any Other Language

There is no list here for Polish, Turkish, Arabic, Japanese or anything else, and one is not needed. Run the translation test on the English entries, apply the structural rules unchanged, drop one register below the formal default, and look for the local equivalent of the two universals: the throat-clearing opener that sets a scene before saying anything, and the tidy summarising close that repeats what the reader just read.

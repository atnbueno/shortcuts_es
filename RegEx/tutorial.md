# Expresiones regulares en Atajos

Las expresiones regulares ("regexes") existen desde mucho antes que los Atajos, así que lo que se aprenda de ellas en Atajos
puede servir en otros sitios. Aunque una expresión regular ("regex") se llama igual en todas partes, hay multiples variantes
de _regex_. Las diferencias entre ellas son sutiles y en este documento se avisará si se usa algo que no sea igual en la 
mayoría de variantes. La Wikipedia en inglés tiene un excelente [resumen de las diferencias entre variantes de _regex_](https://en.wikipedia.org/wiki/Comparison_of_regular-expression_engines#Language_features).

La variante que se usa en la app Atajos es la "UCI Regex" de dicho resumen. La documentación completa (en inglés) de esta
variante se puede encontrar en <http://userguide.icu-project.org/strings/regexp>. Lo más útil en esa URL son las tablas de
metacaracteres y de operadores. Si para probar _regexes_ usas un sitio web o una app, y "ICU" no es uno de las variantes
ofrecidas, selecciona "PCRE" (la más parecida de las variantes populares).

Otra variante relevante aquí es la de JavaScript. Se puede usar en Atajos ejecutando JavaScript en un "Obtener contenido de
página" o equivalente (esto se suele hacer por razones de velocidad). Esta variante está muy bien explicada en MDN:
<https://developer.mozilla.org/es/docs/Web/JavaScript/Guide/Regular_Expressions>. En esta URL lo más útil es la tabla de
compatibilidad en navegadores (para Atajos fíjate en la columna "Safari"). Las diferencias más importantes entre las variantes JavaScript y ICU/PCRE son:

- En JavaScript no se pueden usar capturas con nombre (_named captures_, en inglés)
- En JavaScript no se pueden usar _look-behinds_


_To Be Continued..._ 😅

## Fragmentos a aprovechar en alguna parte

- No usar `.*?` or `(.*?)` al principio o al final de una regex. Pasan cosas raras.

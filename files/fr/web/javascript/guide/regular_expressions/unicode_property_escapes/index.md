---
title: Échappement des propriétés Unicode
slug: Web/JavaScript/Guide/Regular_Expressions/Unicode_Property_Escapes
tags:
  - Expressions rationnelles
  - Expressions régulières
  - Guide
  - JavaScript
  - regex
translation_of: Web/JavaScript/Guide/Regular_Expressions/Unicode_Property_Escapes
original_slug: Web/JavaScript/Guide/Expressions_régulières/Échappement_propriétés_Unicode
---
<p>{{jsSidebar("JavaScript Guide")}}{{draft}}</p>

<p>Les séquences d'échappement pour les propriétés Unicode permettent de distinguer les caractères Unicodes en fonction de leurs propriétés : majuscules, minuscules, symboles mathématiques, ponctuation, etc.</p>

<h2 id="Syntaxe">Syntaxe</h2>

<pre class="brush: js">// Valeurs non-binaires
\p{UnicodePropertyName=<em>ValeurPropriétéUnicode</em>}
\p{UnicodePropertyName}

// Valeurs binaires et non-binaires
\p{UnicodePropertyName}
</pre>

<dl>
 <dt><code>ValeurPropriétéUnicode</code></dt>
 <dd>Une des valeurs listées ci-après. Pour certaines valeurs, le mot-clé <code>NomPropriétéUnicode</code> et le signe égal peuvent être omis.</dd>
</dl>

<h2 id="Valeurs">Valeurs</h2>

<h3 id="Non-binaires">Non-binaires</h3>

<table class="standard-table">
 <thead>
  <tr>
   <th scope="col">Échappements</th>
   <th scope="col">Signification</th>
  </tr>
 </thead>
 <tbody>
  <tr>
   <td><code>\p{LC}<br>
    \p{Cased_Letter}<br>
    \p{UnicodePropertyName=Cased_Letter}</code></td>
   <td>N'importe quelle lettre avec la version minuscule et la version majuscule. Équivalent à <code>\p{Lu}|\p{Ll}|p{Lt}</code>.</td>
  </tr>
  <tr>
   <td><code>\p{Close_Punctuation}<br>
    \p{UnicodePropertyName=Close_Punctuation}</code></td>
   <td></td>
  </tr>
  <tr>
   <td><code>\p{Connector_Punctuation}<br>
    \p{UnicodePropertyName=Connector_Punctuation}</code></td>
   <td></td>
  </tr>
  <tr>
   <td><code>\p{Control}<br>
    \p{UnicodePropertyName=Control}</code></td>
   <td></td>
  </tr>
  <tr>
   <td><code>\p{Currency_Symbol}<br>
    \p{UnicodePropertyName=Currency_Symbol}</code></td>
   <td></td>
  </tr>
  <tr>
   <td><code>\p{Dash_Punctuation}<br>
    \p{UnicodePropertyName=Dash_Punctuation}</code></td>
   <td></td>
  </tr>
  <tr>
   <td><code>\p{Decimal_Number}<br>
    \p{UnicodePropertyName=Decimal_Number}</code></td>
   <td></td>
  </tr>
  <tr>
   <td><code>\p{Enclosing_Mark}<br>
    \p{UnicodePropertyName=Enclosing_Mark}</code></td>
   <td></td>
  </tr>
  <tr>
   <td><code>\p{Final_Punctuation}<br>
    ​​​​​​​\p{UnicodePropertyName=Final_Punctuation}</code></td>
   <td></td>
  </tr>
  <tr>
   <td><code>\p{Format}<br>
    ​​​​​​​\p{UnicodePropertyName=Format}</code></td>
   <td></td>
  </tr>
  <tr>
   <td><code>\p{Initial_Punctuation}<br>
    ​​​​​​​\p{UnicodePropertyName=Initial_Punctuation}</code></td>
   <td></td>
  </tr>
  <tr>
   <td><code>\p{Letter}<br>
    ​​​​​​​\p{UnicodePropertyName=Letter}</code></td>
   <td></td>
  </tr>
  <tr>
   <td><code>\p{Letter_Number}<br>
    ​​​​​​​\p{UnicodePropertyName=Line_Separator}</code></td>
   <td></td>
  </tr>
  <tr>
   <td><code>\p{Lowercase_Letter}<br>
    ​​​​​​​\p{UnicodePropertyName=Lowercase_Letter}</code></td>
   <td></td>
  </tr>
  <tr>
   <td><code>\p{Mark}<br>
    ​​​​​​​\p{UnicodePropertyName=Mark}</code></td>
   <td></td>
  </tr>
  <tr>
   <td><code>\p{Math_Symbol;}<br>
    ​​​​​​​\p{UnicodePropertyName=Math_Symbol}</code></td>
   <td></td>
  </tr>
  <tr>
   <td><code>\p{Modifier_Letter}<br>
    ​​​​​​​\p{UnicodePropertyName=Modifier_Letter}</code></td>
   <td></td>
  </tr>
  <tr>
   <td><code>\p{Modifier_Symbol}<br>
    ​​​​​​​\p{UnicodePropertyName=Modifier_Symbol}</code></td>
   <td></td>
  </tr>
  <tr>
   <td><code>\p{Nonspacing_Mark}<br>
    ​​​​​​​\p{UnicodePropertyName=Nonspacing_Mark}</code></td>
   <td></td>
  </tr>
  <tr>
   <td><code>\p{Number}<br>
    ​​​​​​​\p{UnicodePropertyName=Number}</code></td>
   <td></td>
  </tr>
  <tr>
   <td><code>\p{Open_Punctuation}<br>
    ​​​​​​​\p{UnicodePropertyName=Open_Punctuation}</code></td>
   <td></td>
  </tr>
  <tr>
   <td><code>\p{Other}<br>
    ​​​​​​​\p{UnicodePropertyName=Other_Letter}</code></td>
   <td></td>
  </tr>
  <tr>
   <td><code>\p{Other_Letter}<br>
    ​​​​​​​\p{UnicodePropertyName=Other_Letter}</code></td>
   <td></td>
  </tr>
  <tr>
   <td><code>\p{Other_Number}<br>
    ​​​​​​​\p{UnicodePropertyName=Other_Number}</code></td>
   <td></td>
  </tr>
  <tr>
   <td><code>\p{Other_Punctuation}<br>
    ​​​​​​​\p{UnicodePropertyName=Other_Punctuation}</code></td>
   <td></td>
  </tr>
  <tr>
   <td><code>\p{Paragraph_Separator}<br>
    ​​​​​​​\p{UnicodePropertyName=Paragraph_Separator}</code></td>
   <td></td>
  </tr>
  <tr>
   <td><code>\p{Private_Use}</code>Meaning<br>
    <code>​​​​​​​\p{UnicodePropertyName=Private_Use}</code></td>
   <td></td>
  </tr>
  <tr>
   <td><code>\p{Punctuation}<br>
    ​​​​​​​\p{UnicodePropertyName=Punctuation}</code></td>
   <td></td>
  </tr>
  <tr>
   <td><code>\p{Separator}<br>
    ​​​​​​​\p{UnicodePropertyName=Separator}</code></td>
   <td></td>
  </tr>
  <tr>
   <td><code>\p{Space_Separator}<br>
    ​​​​​​​\p{UnicodePropertyName=Space_Separator}</code></td>
   <td></td>
  </tr>
  <tr>
   <td><code>\p{Spaceing_Mark}<br>
    ​​​​​​​\p{UnicodePropertyName=Spacing_Mark}</code></td>
   <td></td>
  </tr>
  <tr>
   <td><code>\p{Surrogate}<br>
    ​​​​​​​\p{UnicodePropertyName=Surrogate}</code></td>
   <td></td>
  </tr>
  <tr>
   <td><code>\p{Symbol}<br>
    ​​​​​​​\p{UnicodePropertyName=Symbol}</code></td>
   <td></td>
  </tr>
  <tr>
   <td><code>\p{Titlecase_Letter}<br>
    ​​​​​​​\p{UnicodePropertyName=Titlecase_Letter}</code></td>
   <td></td>
  </tr>
  <tr>
   <td><code>\p{Unassigned}<br>
    ​​​​​​​\p{UnicodePropertyName=Unassigned}</code></td>
   <td></td>
  </tr>
  <tr>
   <td><code>\p{Uppercase_Letter}<br>
    ​​​​​​​\p{UnicodePropertyName=UppercaseLetter}</code></td>
   <td></td>
  </tr>
 </tbody>
</table>

<h3 id="Binaires">Binaires</h3>

<table class="standard-table">
 <thead>
  <tr>
   <th scope="col">Échappement</th>
   <th scope="col">Signification</th>
  </tr>
 </thead>
 <tbody>
  <tr>
   <td><code>\p{Alphabetic}</code></td>
   <td></td>
  </tr>
  <tr>
   <td><code>\p{Bidi_Control}</code></td>
   <td></td>
  </tr>
  <tr>
   <td><code>\p{Bidi_Mirrored}</code></td>
   <td></td>
  </tr>
  <tr>
   <td><code>\p{Case_Ignorable}</code></td>
   <td></td>
  </tr>
  <tr>
   <td><code>\p{Cased}</code></td>
   <td></td>
  </tr>
  <tr>
   <td><code>\p{Changes_When_Casefolded}</code></td>
   <td></td>
  </tr>
  <tr>
   <td><code>\p{Changes_When_Casemapped}</code></td>
   <td></td>
  </tr>
  <tr>
   <td><code>\p{Changes_When_Lowercased}</code></td>
   <td></td>
  </tr>
  <tr>
   <td><code>\p{Changes_When_NFKC_Casefolded}</code></td>
   <td></td>
  </tr>
  <tr>
   <td><code>\p{Changes_When_Titlecased}</code></td>
   <td></td>
  </tr>
  <tr>
   <td><code>\p{Changes_When_Uppercased}</code></td>
   <td></td>
  </tr>
  <tr>
   <td><code>\p{Dash}</code></td>
   <td></td>
  </tr>
  <tr>
   <td><code>\p{Default_Ignorable_Code_Point}</code></td>
   <td></td>
  </tr>
  <tr>
   <td><code>\p{Deprecated}</code></td>
   <td></td>
  </tr>
  <tr>
   <td><code>\p{Diacritic}</code></td>
   <td></td>
  </tr>
  <tr>
   <td><code>\p{Emoji}</code></td>
   <td></td>
  </tr>
  <tr>
   <td><code>\p{Emoji_Component}</code></td>
   <td></td>
  </tr>
  <tr>
   <td><code>\p{Emoji_Modifier}</code></td>
   <td></td>
  </tr>
  <tr>
   <td><code>\p{Emoji_Modifier_Base}</code></td>
   <td></td>
  </tr>
  <tr>
   <td><code>\p{Emoji_Presentation}</code></td>
   <td></td>
  </tr>
  <tr>
   <td><code>\p{Extender}</code></td>
   <td></td>
  </tr>
  <tr>
   <td><code>\p{Grapheme_Base}</code></td>
   <td></td>
  </tr>
  <tr>
   <td><code>\p{Grapheme_Extend}</code></td>
   <td></td>
  </tr>
  <tr>
   <td><code>\p{Hex_Digit}</code></td>
   <td></td>
  </tr>
  <tr>
   <td><code>\p{ID_Continue}</code></td>
   <td></td>
  </tr>
  <tr>
   <td><code>\p{ID_Start}</code></td>
   <td></td>
  </tr>
  <tr>
   <td><code>\p{Ideographic}</code></td>
   <td></td>
  </tr>
  <tr>
   <td><code>\p{IDS_Binary_Operator}</code></td>
   <td></td>
  </tr>
  <tr>
   <td><code>\p{IDS_Trinary_Operator}</code></td>
   <td></td>
  </tr>
  <tr>
   <td><code>\p{Join_Control}</code></td>
   <td></td>
  </tr>
  <tr>
   <td><code>\p{Logical_Order_Exception}</code></td>
   <td></td>
  </tr>
  <tr>
   <td><code>\p{Lowercase}</code></td>
   <td></td>
  </tr>
  <tr>
   <td><code>\p{Math}</code></td>
   <td></td>
  </tr>
  <tr>
   <td><code>\p{Noncharacter_Code_Point}</code></td>
   <td></td>
  </tr>
  <tr>
   <td><code>\p{Pattern_Syntax}</code></td>
   <td></td>
  </tr>
  <tr>
   <td><code>\p{Pattern_White_Space}</code></td>
   <td></td>
  </tr>
  <tr>
   <td><code>\p{Quotation_Mark}</code></td>
   <td></td>
  </tr>
  <tr>
   <td><code>\p{Radical}</code></td>
   <td></td>
  </tr>
  <tr>
   <td><code>\p{RegionalIndicator}</code></td>
   <td></td>
  </tr>
  <tr>
   <td><code>\p{Sentence_Terminal}</code></td>
   <td></td>
  </tr>
  <tr>
   <td><code>\p{Soft_Dotted}</code></td>
   <td></td>
  </tr>
  <tr>
   <td><code>\p{Terminal_Punctuation}</code></td>
   <td></td>
  </tr>
  <tr>
   <td><code>\p{Unified_Ideograph}</code></td>
   <td></td>
  </tr>
  <tr>
   <td><code>\p{Uppercase}</code></td>
   <td></td>
  </tr>
  <tr>
   <td><code>\p{Variation_Selector}</code></td>
   <td></td>
  </tr>
  <tr>
   <td><code>\p{White_Space}</code></td>
   <td></td>
  </tr>
  <tr>
   <td><code>\p{XID_Continue}</code></td>
   <td></td>
  </tr>
  <tr>
   <td><code>\p{XID_Start}</code></td>
   <td></td>
  </tr>
 </tbody>
</table>
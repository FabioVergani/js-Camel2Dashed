# js-Camel2Dashed

const camel2dashed=s=>s.replace(/[^A-Z\s][A-Z]/g,t=>[t[0],t[1]].join('-')).toLowerCase();

console.log(camel2dashed('CamelCaseText or CAmelCAseTExt or CAMelCaseTExt '));
//camel-case-text or camel-case-text or camel-case-text

//nb: broken with surrogate pair.

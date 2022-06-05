# Mikhail Lahuta

## Contacts

- Address: Vorovskogo str., Brest, Belarus
- Phone: +375-29-527-80-10
- E-mail: lagutamikhail@gmail.com
- GitHub: [LagutaMikhail](https://github.com/LagutaMikhail/)
- Discord: Mikhail Laguta (@LagutaMikhail)

## About myself: <br/>

I have experience in the field of prevention and liquidation emergency situations.
I am interested in front-end development, and in the future I hope to change my profession.

## Skills:

- HTML
- CSS
- JS Basic

## Code example:

```
module.exports = function check(str, bracketsConfig) {
  let openBrackets =[];
  for (let i=0; i<bracketsConfig.length; i++){
    openBrackets.push(bracketsConfig[i][0])
  };
  let closeBrackets =[];
  for (let i=0; i<bracketsConfig.length; i++){
    closeBrackets.push(bracketsConfig[i][1])
  };

  let s = [];
  for (let i = 0; i<str.length; i++){
    if (s.length==0&&closeBrackets.includes(str[i])){
      return false;
      break;
    }
    else if (openBrackets.includes(str[i])){
      s.push(str[i]);
    }
    else if (closeBrackets.includes(str[i])&&s.length!==0){
      bracketsConfig.forEach(function (item,index) {
        if (item[1] == str[i]&&item[0]==s[s.length-1]){
          s.pop();
        };
      });
      }
    else {
      return false;
      break;
    }
    }
    return s.length==0;
}

```
## Expirience

- [CV project](https://lagutamikhail.github.io/rsschool-cv/cv)

## Education

- Command and engineering institute of the Ministry of Emergency Situations of Belarus - ingeneer of prevention and liquidation emergency situations
- Rolling Scopes Scoll JS/FE stage 0 (in progress)

## Languages:

- Russian - native
- English - A2

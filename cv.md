## Resume 

1. *Artem Katruschenko*
2. *My contacts: email - **katartem200351@gmail.com**, telegram - **@astr02k21**.*
3. *I started studying a web-developing a few month ago, i have a little expierence in programming (JavaScript) i solve tasks on **Codewars** or **HackerRank**. I work with **HTML** and **CSS**. I was developing some web-sites for practicing. I'm going to be a front-end developer in nearest
future.*
4. *So far I only work with **HTML**, **CSS**, **JavaScript** and a little with **Git***
5. *Code example:*  

```

    function getPINs (observed){

        if(observed == undefined || observed == null || observed == '') return ''

        function enumeration(strNum){
            let nums = [['1','2','3'],['4','5','6'],['7','8','9'],[undefined, '0']]

            let i = 0
            let j = 0;

            breaked: for(; i<4; i++){
                j=0
                for(;j<4; j++){
                    if(nums[i][j] == strNum) break breaked;
                }
            }

            function hasser(value1, value2){
                if(nums[value1] && nums[value1][value2]) return nums[value1][value2];
            }

            let keyArr = [hasser(i-1,j), hasser(i, j-1), hasser(i,j), hasser(i, j+1), hasser(i+1, j)];

            return keyArr.filter(item => item != undefined)    

        }

        let observedArr = [...observed];
        let baseArr = enumeration(observedArr[0]);
        let endArr = [];

        for(let i = 1; i < observedArr.length; i++){
            let nowAddEnumeration = enumeration(observedArr[i])
            for(let j = 0; j < baseArr.length; j++){
                for(let k = 0; k < nowAddEnumeration.length; k++){
                    endArr.push(baseArr[j] + nowAddEnumeration[k])
                }
            }
            baseArr = [...endArr];
            endArr = [];
        }
        return baseArr
    }

```  
6. *I don't have work experience. I study from YouTube videos and [The Modern JavaScript Tutorial](https://javascript.info/) or [MDN Web Docs](https://developer.mozilla.org/ru/).*
7. *I'm studying at the college(secondary special education).*
8. *My english level is B1. I have friends foreigners from other countries, i practice english with them, I also studied at an English school*
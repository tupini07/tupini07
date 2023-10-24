## Hi 👋

Thanks for visiting. Here's some nice code

```clojure
(defn multiple-of [p] #(zero? (mod % p)))
(defn sieve [[p & ps]]
  (cons p (lazy-seq (->> ps
                         (remove (multiple-of p))
                         (sieve))))
(take 10 (sieve (iterate inc 2)))
;;=> (2 3 5 7 11 13 17 19 23 29)      
```


<!--
![GitHub stats](https://github-readme-stats.vercel.app/api?username=tupini07&hide=stars&show_icons=true&theme=dracula&count_private=true&show_icons=true)
-->

<!-- ![GitHub languages](https://github-readme-stats.vercel.app/api/top-langs/?username=tupini07&layout=compact&theme=dracula&hide=html,jupyter%20notebook,PLpgSQL,Perl,JavaScript,Lua,Tex) -->



<!--
**tupini07/tupini07** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:

- 🔭 I’m currently working on ...
- 🌱 I’m currently learning ...
- 👯 I’m looking to collaborate on ...
- 🤔 I’m looking for help with ...
- 💬 Ask me about ...
- 📫 How to reach me: ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...
-->

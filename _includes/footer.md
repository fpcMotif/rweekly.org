
<form id="search-form" target="_blank" action="/search.html" method="get">
<label for="search-box"></label>
<input type="text" id="search-box" name="query" placeholder="search">
</form>

<script>
document.getElementById('search-form').addEventListener('submit', function(e){ 
    e.preventDefault();
    var value_search = document.getElementById('search-box').value;
    _paq.push(['trackSiteSearch',
        value_search,
        document.URL,
        0
    ]);
    setTimeout(function(){
       document.location = "https://github.com/rweekly/rweekly.org/search?utf8=%E2%9C%93&q=" + encodeURIComponent(value_search) + "+extension%3Ar+extension%3Amd&type=Code";
    }, 250);
});
</script>

<hr/>
[R](https://www.r-project.org/) is a free software environment for statistical computing and graphics. 

**R Weekly** is openly developed [on GitHub](https://github.com/rweekly/rweekly.org). 

[Twitter @ rweekly_org](https://twitter.com/rweekly_org)

Read more posts on [R-bloggers](http://www.r-bloggers.com).

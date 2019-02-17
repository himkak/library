



<!DOCTYPE html>
<html lang="en" class=" is-copy-enabled is-u2f-enabled">
  <head prefix="og: http://ogp.me/ns# fb: http://ogp.me/ns/fb# object: http://ogp.me/ns/object# article: http://ogp.me/ns/article# profile: http://ogp.me/ns/profile#">
    <meta charset='utf-8'>
    

    <link crossorigin="anonymous" href="https://assets-cdn.github.com/assets/frameworks-b58c080c9d900217a5669b54b61c1609c56789944a064e7a027acd88c75c761e.css" integrity="sha256-tYwIDJ2QAhelZptUthwWCcVniZRKBk56AnrNiMdcdh4=" media="all" rel="stylesheet" />
    <link crossorigin="anonymous" href="https://assets-cdn.github.com/assets/github-13a1b7fab391cd9d7b3827c45eaae67afad4a2a035c59942b0d40f8e75c0e69b.css" integrity="sha256-E6G3+rORzZ17OCfEXqrmevrUoqA1xZlCsNQPjnXA5ps=" media="all" rel="stylesheet" />
    
    
    <link crossorigin="anonymous" href="https://assets-cdn.github.com/assets/site-9e04af73ed9cabf1eb577117611306e88644e59ee7b7b4494d008406599cc7a8.css" integrity="sha256-ngSvc+2cq/HrV3EXYRMG6IZE5Z7nt7RJTQCEBlmcx6g=" media="all" rel="stylesheet" />
    

    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta http-equiv="Content-Language" content="en">
    <meta name="viewport" content="width=device-width">
    
    <title>docker-cheat-sheet/README.md at master · wsargent/docker-cheat-sheet · GitHub</title>
    <link rel="search" type="application/opensearchdescription+xml" href="/opensearch.xml" title="GitHub">
    <link rel="fluid-icon" href="https://github.com/fluidicon.png" title="GitHub">
    <link rel="apple-touch-icon" href="/apple-touch-icon.png">
    <link rel="apple-touch-icon" sizes="57x57" href="/apple-touch-icon-57x57.png">
    <link rel="apple-touch-icon" sizes="60x60" href="/apple-touch-icon-60x60.png">
    <link rel="apple-touch-icon" sizes="72x72" href="/apple-touch-icon-72x72.png">
    <link rel="apple-touch-icon" sizes="76x76" href="/apple-touch-icon-76x76.png">
    <link rel="apple-touch-icon" sizes="114x114" href="/apple-touch-icon-114x114.png">
    <link rel="apple-touch-icon" sizes="120x120" href="/apple-touch-icon-120x120.png">
    <link rel="apple-touch-icon" sizes="144x144" href="/apple-touch-icon-144x144.png">
    <link rel="apple-touch-icon" sizes="152x152" href="/apple-touch-icon-152x152.png">
    <link rel="apple-touch-icon" sizes="180x180" href="/apple-touch-icon-180x180.png">
    <meta property="fb:app_id" content="1401488693436528">

      <meta content="https://avatars1.githubusercontent.com/u/71236?v=3&amp;s=400" name="twitter:image:src" /><meta content="@github" name="twitter:site" /><meta content="summary" name="twitter:card" /><meta content="wsargent/docker-cheat-sheet" name="twitter:title" /><meta content="docker-cheat-sheet - Docker Cheat Sheet" name="twitter:description" />
      <meta content="https://avatars1.githubusercontent.com/u/71236?v=3&amp;s=400" property="og:image" /><meta content="GitHub" property="og:site_name" /><meta content="object" property="og:type" /><meta content="wsargent/docker-cheat-sheet" property="og:title" /><meta content="https://github.com/wsargent/docker-cheat-sheet" property="og:url" /><meta content="docker-cheat-sheet - Docker Cheat Sheet" property="og:description" />
      <meta name="browser-stats-url" content="https://api.github.com/_private/browser/stats">
    <meta name="browser-errors-url" content="https://api.github.com/_private/browser/errors">
    <link rel="assets" href="https://assets-cdn.github.com/">
    
    <meta name="pjax-timeout" content="1000">
    
    <meta name="request-id" content="0E8E2142:7586:74487D3:58230CE6" data-pjax-transient>

    <meta name="msapplication-TileImage" content="/windows-tile.png">
    <meta name="msapplication-TileColor" content="#ffffff">
    <meta name="selected-link" value="repo_source" data-pjax-transient>

    <meta name="google-site-verification" content="KT5gs8h0wvaagLKAVWq8bbeNwnZZK1r1XQysX3xurLU">
<meta name="google-site-verification" content="ZzhVyEFwb7w3e0-uOTltm8Jsck2F5StVihD0exw2fsA">
    <meta name="google-analytics" content="UA-3769691-2">

<meta content="collector.githubapp.com" name="octolytics-host" /><meta content="github" name="octolytics-app-id" /><meta content="0E8E2142:7586:74487D3:58230CE6" name="octolytics-dimension-request_id" />
<meta content="/&lt;user-name&gt;/&lt;repo-name&gt;/blob/show" data-pjax-transient="true" name="analytics-location" />



  <meta class="js-ga-set" name="dimension1" content="Logged Out">



        <meta name="hostname" content="github.com">
    <meta name="user-login" content="">

        <meta name="expected-hostname" content="github.com">
      <meta name="js-proxy-site-detection-payload" content="YzI5MjNkYjVjMTJkZTE0OGNiM2NhZWMwMGE3NmZmODQ2ODhjM2RhZjE1NjFlYjVhNTZlY2YyN2I5NGI2ZDc0Ynx7InJlbW90ZV9hZGRyZXNzIjoiMTQuMTQyLjMzLjY2IiwicmVxdWVzdF9pZCI6IjBFOEUyMTQyOjc1ODY6NzQ0ODdEMzo1ODIzMENFNiIsInRpbWVzdGFtcCI6MTQ3ODY5MjA3MCwiaG9zdCI6ImdpdGh1Yi5jb20ifQ==">


      <link rel="mask-icon" href="https://assets-cdn.github.com/pinned-octocat.svg" color="#4078c0">
      <link rel="icon" type="image/x-icon" href="https://assets-cdn.github.com/favicon.ico">

    <meta name="html-safe-nonce" content="7f3a7217296cb4bc541d8871f76ffa5510ab82c6">
    <meta content="23944c3b476425435d5983a2d5d8b2ce8657ae80" name="form-nonce" />

    <meta http-equiv="x-pjax-version" content="439fe676687bceadb3356ba20a64c3bd">
    

      
  <meta name="description" content="docker-cheat-sheet - Docker Cheat Sheet">
  <meta name="go-import" content="github.com/wsargent/docker-cheat-sheet git https://github.com/wsargent/docker-cheat-sheet.git">

  <meta content="71236" name="octolytics-dimension-user_id" /><meta content="wsargent" name="octolytics-dimension-user_login" /><meta content="22657662" name="octolytics-dimension-repository_id" /><meta content="wsargent/docker-cheat-sheet" name="octolytics-dimension-repository_nwo" /><meta content="true" name="octolytics-dimension-repository_public" /><meta content="false" name="octolytics-dimension-repository_is_fork" /><meta content="22657662" name="octolytics-dimension-repository_network_root_id" /><meta content="wsargent/docker-cheat-sheet" name="octolytics-dimension-repository_network_root_nwo" />
  <link href="https://github.com/wsargent/docker-cheat-sheet/commits/master.atom" rel="alternate" title="Recent Commits to docker-cheat-sheet:master" type="application/atom+xml">


      <link rel="canonical" href="https://github.com/wsargent/docker-cheat-sheet/blob/master/README.md" data-pjax-transient>
  </head>


  <body class="logged-out  env-production windows vis-public page-blob">
    <div id="js-pjax-loader-bar" class="pjax-loader-bar"><div class="progress"></div></div>
    <a href="#start-of-content" tabindex="1" class="accessibility-aid js-skip-to-content">Skip to content</a>

    
    
    



          <header class="site-header js-details-container" role="banner">
  <div class="container-responsive">
    <a class="header-logo-invertocat" href="https://github.com/" aria-label="Homepage" data-ga-click="(Logged out) Header, go to homepage, icon:logo-wordmark">
      <svg aria-hidden="true" class="octicon octicon-mark-github" height="32" version="1.1" viewBox="0 0 16 16" width="32"><path fill-rule="evenodd" d="M8 0C3.58 0 0 3.58 0 8c0 3.54 2.29 6.53 5.47 7.59.4.07.55-.17.55-.38 0-.19-.01-.82-.01-1.49-2.01.37-2.53-.49-2.69-.94-.09-.23-.48-.94-.82-1.13-.28-.15-.68-.52-.01-.53.63-.01 1.08.58 1.23.82.72 1.21 1.87.87 2.33.66.07-.52.28-.87.51-1.07-1.78-.2-3.64-.89-3.64-3.95 0-.87.31-1.59.82-2.15-.08-.2-.36-1.02.08-2.12 0 0 .67-.21 2.2.82.64-.18 1.32-.27 2-.27.68 0 1.36.09 2 .27 1.53-1.04 2.2-.82 2.2-.82.44 1.1.16 1.92.08 2.12.51.56.82 1.27.82 2.15 0 3.07-1.87 3.75-3.65 3.95.29.25.54.73.54 1.48 0 1.07-.01 1.93-.01 2.2 0 .21.15.46.55.38A8.013 8.013 0 0 0 16 8c0-4.42-3.58-8-8-8z"/></svg>
    </a>

    <button class="btn-link float-right site-header-toggle js-details-target" type="button" aria-label="Toggle navigation">
      <svg aria-hidden="true" class="octicon octicon-three-bars" height="24" version="1.1" viewBox="0 0 12 16" width="18"><path fill-rule="evenodd" d="M11.41 9H.59C0 9 0 8.59 0 8c0-.59 0-1 .59-1H11.4c.59 0 .59.41.59 1 0 .59 0 1-.59 1h.01zm0-4H.59C0 5 0 4.59 0 4c0-.59 0-1 .59-1H11.4c.59 0 .59.41.59 1 0 .59 0 1-.59 1h.01zM.59 11H11.4c.59 0 .59.41.59 1 0 .59 0 1-.59 1H.59C0 13 0 12.59 0 12c0-.59 0-1 .59-1z"/></svg>
    </button>

    <div class="site-header-menu">
      <nav class="site-header-nav site-header-nav-main">
        <a href="/personal" class="js-selected-navigation-item nav-item nav-item-personal" data-ga-click="Header, click, Nav menu - item:personal" data-selected-links="/personal /personal">
          Personal
</a>        <a href="/open-source" class="js-selected-navigation-item nav-item nav-item-opensource" data-ga-click="Header, click, Nav menu - item:opensource" data-selected-links="/open-source /open-source">
          Open source
</a>        <a href="/business" class="js-selected-navigation-item nav-item nav-item-business" data-ga-click="Header, click, Nav menu - item:business" data-selected-links="/business /business/partners /business/features /business/customers /business">
          Business
</a>        <a href="/explore" class="js-selected-navigation-item nav-item nav-item-explore" data-ga-click="Header, click, Nav menu - item:explore" data-selected-links="/explore /trending /trending/developers /integrations /integrations/feature/code /integrations/feature/collaborate /integrations/feature/ship /showcases /explore">
          Explore
</a>      </nav>

      <div class="site-header-actions">
            <a class="btn btn-primary site-header-actions-btn" href="/join?source=header-repo" data-ga-click="(Logged out) Header, clicked Sign up, text:sign-up">Sign up</a>
          <a class="btn site-header-actions-btn mr-1" href="/login?return_to=%2Fwsargent%2Fdocker-cheat-sheet%2Fblob%2Fmaster%2FREADME.md" data-ga-click="(Logged out) Header, clicked Sign in, text:sign-in">Sign in</a>
      </div>

        <nav class="site-header-nav site-header-nav-secondary mr-md-3">
          <a class="nav-item" href="/pricing">Pricing</a>
          <a class="nav-item" href="/blog">Blog</a>
          <a class="nav-item" href="https://help.github.com">Support</a>
          <a class="nav-item header-search-link" href="https://github.com/search">Search GitHub</a>
              <div class="header-search scoped-search site-scoped-search js-site-search" role="search">
  <!-- '"` --><!-- </textarea></xmp> --></option></form><form accept-charset="UTF-8" action="/wsargent/docker-cheat-sheet/search" class="js-site-search-form" data-scoped-search-url="/wsargent/docker-cheat-sheet/search" data-unscoped-search-url="/search" method="get"><div style="margin:0;padding:0;display:inline"><input name="utf8" type="hidden" value="&#x2713;" /></div>
    <label class="form-control header-search-wrapper js-chromeless-input-container">
      <div class="header-search-scope">This repository</div>
      <input type="text"
        class="form-control header-search-input js-site-search-focus js-site-search-field is-clearable"
        data-hotkey="s"
        name="q"
        placeholder="Search"
        aria-label="Search this repository"
        data-unscoped-placeholder="Search GitHub"
        data-scoped-placeholder="Search"
        autocapitalize="off">
    </label>
</form></div>

        </nav>
    </div>
  </div>
</header>



    <div id="start-of-content" class="accessibility-aid"></div>

      <div id="js-flash-container">
</div>


    <div role="main">
        <div itemscope itemtype="http://schema.org/SoftwareSourceCode">
    <div id="js-repo-pjax-container" data-pjax-container>
      
<div class="pagehead repohead instapaper_ignore readability-menu experiment-repo-nav">
  <div class="container repohead-details-container">

    

<ul class="pagehead-actions">

  <li>
      <a href="/login?return_to=%2Fwsargent%2Fdocker-cheat-sheet"
    class="btn btn-sm btn-with-count tooltipped tooltipped-n"
    aria-label="You must be signed in to watch a repository" rel="nofollow">
    <svg aria-hidden="true" class="octicon octicon-eye" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M8.06 2C3 2 0 8 0 8s3 6 8.06 6C13 14 16 8 16 8s-3-6-7.94-6zM8 12c-2.2 0-4-1.78-4-4 0-2.2 1.8-4 4-4 2.22 0 4 1.8 4 4 0 2.22-1.78 4-4 4zm2-4c0 1.11-.89 2-2 2-1.11 0-2-.89-2-2 0-1.11.89-2 2-2 1.11 0 2 .89 2 2z"/></svg>
    Watch
  </a>
  <a class="social-count" href="/wsargent/docker-cheat-sheet/watchers"
     aria-label="462 users are watching this repository">
    462
  </a>

  </li>

  <li>
      <a href="/login?return_to=%2Fwsargent%2Fdocker-cheat-sheet"
    class="btn btn-sm btn-with-count tooltipped tooltipped-n"
    aria-label="You must be signed in to star a repository" rel="nofollow">
    <svg aria-hidden="true" class="octicon octicon-star" height="16" version="1.1" viewBox="0 0 14 16" width="14"><path fill-rule="evenodd" d="M14 6l-4.9-.64L7 1 4.9 5.36 0 6l3.6 3.26L2.67 14 7 11.67 11.33 14l-.93-4.74z"/></svg>
    Star
  </a>

    <a class="social-count js-social-count" href="/wsargent/docker-cheat-sheet/stargazers"
      aria-label="8064 users starred this repository">
      8,064
    </a>

  </li>

  <li>
      <a href="/login?return_to=%2Fwsargent%2Fdocker-cheat-sheet"
        class="btn btn-sm btn-with-count tooltipped tooltipped-n"
        aria-label="You must be signed in to fork a repository" rel="nofollow">
        <svg aria-hidden="true" class="octicon octicon-repo-forked" height="16" version="1.1" viewBox="0 0 10 16" width="10"><path fill-rule="evenodd" d="M8 1a1.993 1.993 0 0 0-1 3.72V6L5 8 3 6V4.72A1.993 1.993 0 0 0 2 1a1.993 1.993 0 0 0-1 3.72V6.5l3 3v1.78A1.993 1.993 0 0 0 5 15a1.993 1.993 0 0 0 1-3.72V9.5l3-3V4.72A1.993 1.993 0 0 0 8 1zM2 4.2C1.34 4.2.8 3.65.8 3c0-.65.55-1.2 1.2-1.2.65 0 1.2.55 1.2 1.2 0 .65-.55 1.2-1.2 1.2zm3 10c-.66 0-1.2-.55-1.2-1.2 0-.65.55-1.2 1.2-1.2.65 0 1.2.55 1.2 1.2 0 .65-.55 1.2-1.2 1.2zm3-10c-.66 0-1.2-.55-1.2-1.2 0-.65.55-1.2 1.2-1.2.65 0 1.2.55 1.2 1.2 0 .65-.55 1.2-1.2 1.2z"/></svg>
        Fork
      </a>

    <a href="/wsargent/docker-cheat-sheet/network" class="social-count"
       aria-label="1262 users are forked this repository">
      1,262
    </a>
  </li>
</ul>

    <h1 class="public ">
  <svg aria-hidden="true" class="octicon octicon-repo" height="16" version="1.1" viewBox="0 0 12 16" width="12"><path fill-rule="evenodd" d="M4 9H3V8h1v1zm0-3H3v1h1V6zm0-2H3v1h1V4zm0-2H3v1h1V2zm8-1v12c0 .55-.45 1-1 1H6v2l-1.5-1.5L3 16v-2H1c-.55 0-1-.45-1-1V1c0-.55.45-1 1-1h10c.55 0 1 .45 1 1zm-1 10H1v2h2v-1h3v1h5v-2zm0-10H2v9h9V1z"/></svg>
  <span class="author" itemprop="author"><a href="/wsargent" class="url fn" rel="author">wsargent</a></span><!--
--><span class="path-divider">/</span><!--
--><strong itemprop="name"><a href="/wsargent/docker-cheat-sheet" data-pjax="#js-repo-pjax-container">docker-cheat-sheet</a></strong>

</h1>

  </div>
  <div class="container">
    
<nav class="reponav js-repo-nav js-sidenav-container-pjax"
     itemscope
     itemtype="http://schema.org/BreadcrumbList"
     role="navigation"
     data-pjax="#js-repo-pjax-container">

  <span itemscope itemtype="http://schema.org/ListItem" itemprop="itemListElement">
    <a href="/wsargent/docker-cheat-sheet" aria-selected="true" class="js-selected-navigation-item selected reponav-item" data-hotkey="g c" data-selected-links="repo_source repo_downloads repo_commits repo_releases repo_tags repo_branches /wsargent/docker-cheat-sheet" itemprop="url">
      <svg aria-hidden="true" class="octicon octicon-code" height="16" version="1.1" viewBox="0 0 14 16" width="14"><path fill-rule="evenodd" d="M9.5 3L8 4.5 11.5 8 8 11.5 9.5 13 14 8 9.5 3zm-5 0L0 8l4.5 5L6 11.5 2.5 8 6 4.5 4.5 3z"/></svg>
      <span itemprop="name">Code</span>
      <meta itemprop="position" content="1">
</a>  </span>

    <span itemscope itemtype="http://schema.org/ListItem" itemprop="itemListElement">
      <a href="/wsargent/docker-cheat-sheet/issues" class="js-selected-navigation-item reponav-item" data-hotkey="g i" data-selected-links="repo_issues repo_labels repo_milestones /wsargent/docker-cheat-sheet/issues" itemprop="url">
        <svg aria-hidden="true" class="octicon octicon-issue-opened" height="16" version="1.1" viewBox="0 0 14 16" width="14"><path fill-rule="evenodd" d="M7 2.3c3.14 0 5.7 2.56 5.7 5.7s-2.56 5.7-5.7 5.7A5.71 5.71 0 0 1 1.3 8c0-3.14 2.56-5.7 5.7-5.7zM7 1C3.14 1 0 4.14 0 8s3.14 7 7 7 7-3.14 7-7-3.14-7-7-7zm1 3H6v5h2V4zm0 6H6v2h2v-2z"/></svg>
        <span itemprop="name">Issues</span>
        <span class="counter">0</span>
        <meta itemprop="position" content="2">
</a>    </span>

  <span itemscope itemtype="http://schema.org/ListItem" itemprop="itemListElement">
    <a href="/wsargent/docker-cheat-sheet/pulls" class="js-selected-navigation-item reponav-item" data-hotkey="g p" data-selected-links="repo_pulls /wsargent/docker-cheat-sheet/pulls" itemprop="url">
      <svg aria-hidden="true" class="octicon octicon-git-pull-request" height="16" version="1.1" viewBox="0 0 12 16" width="12"><path fill-rule="evenodd" d="M11 11.28V5c-.03-.78-.34-1.47-.94-2.06C9.46 2.35 8.78 2.03 8 2H7V0L4 3l3 3V4h1c.27.02.48.11.69.31.21.2.3.42.31.69v6.28A1.993 1.993 0 0 0 10 15a1.993 1.993 0 0 0 1-3.72zm-1 2.92c-.66 0-1.2-.55-1.2-1.2 0-.65.55-1.2 1.2-1.2.65 0 1.2.55 1.2 1.2 0 .65-.55 1.2-1.2 1.2zM4 3c0-1.11-.89-2-2-2a1.993 1.993 0 0 0-1 3.72v6.56A1.993 1.993 0 0 0 2 15a1.993 1.993 0 0 0 1-3.72V4.72c.59-.34 1-.98 1-1.72zm-.8 10c0 .66-.55 1.2-1.2 1.2-.65 0-1.2-.55-1.2-1.2 0-.65.55-1.2 1.2-1.2.65 0 1.2.55 1.2 1.2zM2 4.2C1.34 4.2.8 3.65.8 3c0-.65.55-1.2 1.2-1.2.65 0 1.2.55 1.2 1.2 0 .65-.55 1.2-1.2 1.2z"/></svg>
      <span itemprop="name">Pull requests</span>
      <span class="counter">4</span>
      <meta itemprop="position" content="3">
</a>  </span>

  <a href="/wsargent/docker-cheat-sheet/projects" class="js-selected-navigation-item reponav-item" data-selected-links="repo_projects new_repo_project repo_project /wsargent/docker-cheat-sheet/projects">
    <svg aria-hidden="true" class="octicon octicon-project" height="16" version="1.1" viewBox="0 0 15 16" width="15"><path fill-rule="evenodd" d="M10 12h3V2h-3v10zm-4-2h3V2H6v8zm-4 4h3V2H2v12zm-1 1h13V1H1v14zM14 0H1a1 1 0 0 0-1 1v14a1 1 0 0 0 1 1h13a1 1 0 0 0 1-1V1a1 1 0 0 0-1-1z"/></svg>
    Projects
    <span class="counter">0</span>
</a>


  <a href="/wsargent/docker-cheat-sheet/pulse" class="js-selected-navigation-item reponav-item" data-selected-links="pulse /wsargent/docker-cheat-sheet/pulse">
    <svg aria-hidden="true" class="octicon octicon-pulse" height="16" version="1.1" viewBox="0 0 14 16" width="14"><path fill-rule="evenodd" d="M11.5 8L8.8 5.4 6.6 8.5 5.5 1.6 2.38 8H0v2h3.6l.9-1.8.9 5.4L9 8.5l1.6 1.5H14V8z"/></svg>
    Pulse
</a>
  <a href="/wsargent/docker-cheat-sheet/graphs" class="js-selected-navigation-item reponav-item" data-selected-links="repo_graphs repo_contributors /wsargent/docker-cheat-sheet/graphs">
    <svg aria-hidden="true" class="octicon octicon-graph" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M16 14v1H0V0h1v14h15zM5 13H3V8h2v5zm4 0H7V3h2v10zm4 0h-2V6h2v7z"/></svg>
    Graphs
</a>

</nav>

  </div>
</div>

<div class="container new-discussion-timeline experiment-repo-nav">
  <div class="repository-content">

    

<a href="/wsargent/docker-cheat-sheet/blob/eb996d5b6e10f36a6e22bce47b9c72c71d2ff38d/README.md" class="d-none js-permalink-shortcut" data-hotkey="y">Permalink</a>

<!-- blob contrib key: blob_contributors:v21:eb0ca6376673d29616d95cad44410cff -->

<div class="file-navigation js-zeroclipboard-container">
  
<div class="select-menu branch-select-menu js-menu-container js-select-menu float-left">
  <button class="btn btn-sm select-menu-button js-menu-target css-truncate" data-hotkey="w"
    
    type="button" aria-label="Switch branches or tags" tabindex="0" aria-haspopup="true">
    <i>Branch:</i>
    <span class="js-select-button css-truncate-target">master</span>
  </button>

  <div class="select-menu-modal-holder js-menu-content js-navigation-container" data-pjax aria-hidden="true">

    <div class="select-menu-modal">
      <div class="select-menu-header">
        <svg aria-label="Close" class="octicon octicon-x js-menu-close" height="16" role="img" version="1.1" viewBox="0 0 12 16" width="12"><path fill-rule="evenodd" d="M7.48 8l3.75 3.75-1.48 1.48L6 9.48l-3.75 3.75-1.48-1.48L4.52 8 .77 4.25l1.48-1.48L6 6.52l3.75-3.75 1.48 1.48z"/></svg>
        <span class="select-menu-title">Switch branches/tags</span>
      </div>

      <div class="select-menu-filters">
        <div class="select-menu-text-filter">
          <input type="text" aria-label="Filter branches/tags" id="context-commitish-filter-field" class="form-control js-filterable-field js-navigation-enable" placeholder="Filter branches/tags">
        </div>
        <div class="select-menu-tabs">
          <ul>
            <li class="select-menu-tab">
              <a href="#" data-tab-filter="branches" data-filter-placeholder="Filter branches/tags" class="js-select-menu-tab" role="tab">Branches</a>
            </li>
            <li class="select-menu-tab">
              <a href="#" data-tab-filter="tags" data-filter-placeholder="Find a tag…" class="js-select-menu-tab" role="tab">Tags</a>
            </li>
          </ul>
        </div>
      </div>

      <div class="select-menu-list select-menu-tab-bucket js-select-menu-tab-bucket" data-tab-filter="branches" role="menu">

        <div data-filterable-for="context-commitish-filter-field" data-filterable-type="substring">


            <a class="select-menu-item js-navigation-item js-navigation-open selected"
               href="/wsargent/docker-cheat-sheet/blob/master/README.md"
               data-name="master"
               data-skip-pjax="true"
               rel="nofollow">
              <svg aria-hidden="true" class="octicon octicon-check select-menu-item-icon" height="16" version="1.1" viewBox="0 0 12 16" width="12"><path fill-rule="evenodd" d="M12 5l-8 8-4-4 1.5-1.5L4 10l6.5-6.5z"/></svg>
              <span class="select-menu-item-text css-truncate-target js-select-menu-filter-text">
                master
              </span>
            </a>
            <a class="select-menu-item js-navigation-item js-navigation-open "
               href="/wsargent/docker-cheat-sheet/blob/update-security-section/README.md"
               data-name="update-security-section"
               data-skip-pjax="true"
               rel="nofollow">
              <svg aria-hidden="true" class="octicon octicon-check select-menu-item-icon" height="16" version="1.1" viewBox="0 0 12 16" width="12"><path fill-rule="evenodd" d="M12 5l-8 8-4-4 1.5-1.5L4 10l6.5-6.5z"/></svg>
              <span class="select-menu-item-text css-truncate-target js-select-menu-filter-text">
                update-security-section
              </span>
            </a>
        </div>

          <div class="select-menu-no-results">Nothing to show</div>
      </div>

      <div class="select-menu-list select-menu-tab-bucket js-select-menu-tab-bucket" data-tab-filter="tags">
        <div data-filterable-for="context-commitish-filter-field" data-filterable-type="substring">


        </div>

        <div class="select-menu-no-results">Nothing to show</div>
      </div>

    </div>
  </div>
</div>

  <div class="BtnGroup float-right">
    <a href="/wsargent/docker-cheat-sheet/find/master"
          class="js-pjax-capture-input btn btn-sm BtnGroup-item"
          data-pjax
          data-hotkey="t">
      Find file
    </a>
    <button aria-label="Copy file path to clipboard" class="js-zeroclipboard btn btn-sm BtnGroup-item tooltipped tooltipped-s" data-copied-hint="Copied!" type="button">Copy path</button>
  </div>
  <div class="breadcrumb js-zeroclipboard-target">
    <span class="repo-root js-repo-root"><span class="js-path-segment"><a href="/wsargent/docker-cheat-sheet"><span>docker-cheat-sheet</span></a></span></span><span class="separator">/</span><strong class="final-path">README.md</strong>
  </div>
</div>


  <div class="commit-tease">
      <span class="float-right">
        <a class="commit-tease-sha" href="/wsargent/docker-cheat-sheet/commit/7c210cc4c3e5b55688f1aa3d2d50c24cef9c48e5" data-pjax>
          7c210cc
        </a>
        <relative-time datetime="2016-10-30T22:43:21Z">Oct 31, 2016</relative-time>
      </span>
      <div>
        <img alt="@jghaines" class="avatar" height="20" src="https://avatars0.githubusercontent.com/u/977737?v=3&amp;s=40" width="20" />
        <a href="/jghaines" class="user-mention" rel="contributor">jghaines</a>
          <a href="/wsargent/docker-cheat-sheet/commit/7c210cc4c3e5b55688f1aa3d2d50c24cef9c48e5" class="message" data-pjax="true" title="Why -&gt; Why Docker

This section is about why docker, not about why a cheat sheet.">Why -&gt; Why Docker</a>
      </div>

    <div class="commit-tease-contributors">
      <button type="button" class="btn-link muted-link contributors-toggle" data-facebox="#blob_contributors_box">
        <strong>63</strong>
         contributors
      </button>
          <a class="avatar-link tooltipped tooltipped-s" aria-label="wsargent" href="/wsargent/docker-cheat-sheet/commits/master/README.md?author=wsargent"><img alt="@wsargent" class="avatar" height="20" src="https://avatars2.githubusercontent.com/u/71236?v=3&amp;s=40" width="20" /> </a>
    <a class="avatar-link tooltipped tooltipped-s" aria-label="amirbawab" href="/wsargent/docker-cheat-sheet/commits/master/README.md?author=amirbawab"><img alt="@amirbawab" class="avatar" height="20" src="https://avatars3.githubusercontent.com/u/6259858?v=3&amp;s=40" width="20" /> </a>
    <a class="avatar-link tooltipped tooltipped-s" aria-label="jalateras" href="/wsargent/docker-cheat-sheet/commits/master/README.md?author=jalateras"><img alt="@jalateras" class="avatar" height="20" src="https://avatars1.githubusercontent.com/u/1454089?v=3&amp;s=40" width="20" /> </a>
    <a class="avatar-link tooltipped tooltipped-s" aria-label="ReadmeCritic" href="/wsargent/docker-cheat-sheet/commits/master/README.md?author=ReadmeCritic"><img alt="@ReadmeCritic" class="avatar" height="20" src="https://avatars0.githubusercontent.com/u/15367484?v=3&amp;s=40" width="20" /> </a>
    <a class="avatar-link tooltipped tooltipped-s" aria-label="outcoldman" href="/wsargent/docker-cheat-sheet/commits/master/README.md?author=outcoldman"><img alt="@outcoldman" class="avatar" height="20" src="https://avatars2.githubusercontent.com/u/597158?v=3&amp;s=40" width="20" /> </a>
    <a class="avatar-link tooltipped tooltipped-s" aria-label="dkhamsing" href="/wsargent/docker-cheat-sheet/commits/master/README.md?author=dkhamsing"><img alt="@dkhamsing" class="avatar" height="20" src="https://avatars2.githubusercontent.com/u/4723115?v=3&amp;s=40" width="20" /> </a>
    <a class="avatar-link tooltipped tooltipped-s" aria-label="tuksik" href="/wsargent/docker-cheat-sheet/commits/master/README.md?author=tuksik"><img alt="@tuksik" class="avatar" height="20" src="https://avatars3.githubusercontent.com/u/386140?v=3&amp;s=40" width="20" /> </a>
    <a class="avatar-link tooltipped tooltipped-s" aria-label="ttres" href="/wsargent/docker-cheat-sheet/commits/master/README.md?author=ttres"><img alt="@ttres" class="avatar" height="20" src="https://avatars1.githubusercontent.com/u/493551?v=3&amp;s=40" width="20" /> </a>
    <a class="avatar-link tooltipped tooltipped-s" aria-label="thorstenc" href="/wsargent/docker-cheat-sheet/commits/master/README.md?author=thorstenc"><img alt="@thorstenc" class="avatar" height="20" src="https://avatars3.githubusercontent.com/u/869096?v=3&amp;s=40" width="20" /> </a>
    <a class="avatar-link tooltipped tooltipped-s" aria-label="vdemario" href="/wsargent/docker-cheat-sheet/commits/master/README.md?author=vdemario"><img alt="@vdemario" class="avatar" height="20" src="https://avatars1.githubusercontent.com/u/6087424?v=3&amp;s=40" width="20" /> </a>
    <a class="avatar-link tooltipped tooltipped-s" aria-label="lherrera" href="/wsargent/docker-cheat-sheet/commits/master/README.md?author=lherrera"><img alt="@lherrera" class="avatar" height="20" src="https://avatars1.githubusercontent.com/u/2963309?v=3&amp;s=40" width="20" /> </a>
    <a class="avatar-link tooltipped tooltipped-s" aria-label="manycoding" href="/wsargent/docker-cheat-sheet/commits/master/README.md?author=manycoding"><img alt="@manycoding" class="avatar" height="20" src="https://avatars2.githubusercontent.com/u/10396557?v=3&amp;s=40" width="20" /> </a>
    <a class="avatar-link tooltipped tooltipped-s" aria-label="mariorez" href="/wsargent/docker-cheat-sheet/commits/master/README.md?author=mariorez"><img alt="@mariorez" class="avatar" height="20" src="https://avatars2.githubusercontent.com/u/197228?v=3&amp;s=40" width="20" /> </a>
    <a class="avatar-link tooltipped tooltipped-s" aria-label="kxxoling" href="/wsargent/docker-cheat-sheet/commits/master/README.md?author=kxxoling"><img alt="@kxxoling" class="avatar" height="20" src="https://avatars2.githubusercontent.com/u/1227139?v=3&amp;s=40" width="20" /> </a>
    <a class="avatar-link tooltipped tooltipped-s" aria-label="rmetzler" href="/wsargent/docker-cheat-sheet/commits/master/README.md?author=rmetzler"><img alt="@rmetzler" class="avatar" height="20" src="https://avatars3.githubusercontent.com/u/58824?v=3&amp;s=40" width="20" /> </a>
    <a class="avatar-link tooltipped tooltipped-s" aria-label="PetrGlad" href="/wsargent/docker-cheat-sheet/commits/master/README.md?author=PetrGlad"><img alt="@PetrGlad" class="avatar" height="20" src="https://avatars0.githubusercontent.com/u/124476?v=3&amp;s=40" width="20" /> </a>
    <a class="avatar-link tooltipped tooltipped-s" aria-label="ming13" href="/wsargent/docker-cheat-sheet/commits/master/README.md?author=ming13"><img alt="@ming13" class="avatar" height="20" src="https://avatars0.githubusercontent.com/u/200401?v=3&amp;s=40" width="20" /> </a>
    <a class="avatar-link tooltipped tooltipped-s" aria-label="vorburger" href="/wsargent/docker-cheat-sheet/commits/master/README.md?author=vorburger"><img alt="@vorburger" class="avatar" height="20" src="https://avatars1.githubusercontent.com/u/298598?v=3&amp;s=40" width="20" /> </a>
    <a class="avatar-link tooltipped tooltipped-s" aria-label="kherrick" href="/wsargent/docker-cheat-sheet/commits/master/README.md?author=kherrick"><img alt="@kherrick" class="avatar" height="20" src="https://avatars2.githubusercontent.com/u/3065761?v=3&amp;s=40" width="20" /> </a>
    <a class="avatar-link tooltipped tooltipped-s" aria-label="berekuk" href="/wsargent/docker-cheat-sheet/commits/master/README.md?author=berekuk"><img alt="@berekuk" class="avatar" height="20" src="https://avatars3.githubusercontent.com/u/89368?v=3&amp;s=40" width="20" /> </a>
    <a class="avatar-link tooltipped tooltipped-s" aria-label="mattreyuk" href="/wsargent/docker-cheat-sheet/commits/master/README.md?author=mattreyuk"><img alt="@mattreyuk" class="avatar" height="20" src="https://avatars0.githubusercontent.com/u/926405?v=3&amp;s=40" width="20" /> </a>
    <a class="avatar-link tooltipped tooltipped-s" aria-label="Secathor" href="/wsargent/docker-cheat-sheet/commits/master/README.md?author=Secathor"><img alt="@Secathor" class="avatar" height="20" src="https://avatars1.githubusercontent.com/u/107411?v=3&amp;s=40" width="20" /> </a>
    <a class="avatar-link tooltipped tooltipped-s" aria-label="Skamander" href="/wsargent/docker-cheat-sheet/commits/master/README.md?author=Skamander"><img alt="@Skamander" class="avatar" height="20" src="https://avatars1.githubusercontent.com/u/4005707?v=3&amp;s=40" width="20" /> </a>
    <a class="avatar-link tooltipped tooltipped-s" aria-label="cschneider4711" href="/wsargent/docker-cheat-sheet/commits/master/README.md?author=cschneider4711"><img alt="@cschneider4711" class="avatar" height="20" src="https://avatars1.githubusercontent.com/u/6897328?v=3&amp;s=40" width="20" /> </a>
    <a class="avatar-link tooltipped tooltipped-s" aria-label="LouisVN" href="/wsargent/docker-cheat-sheet/commits/master/README.md?author=LouisVN"><img alt="@LouisVN" class="avatar" height="20" src="https://avatars3.githubusercontent.com/u/18465316?v=3&amp;s=40" width="20" /> </a>
    <a class="avatar-link tooltipped tooltipped-s" aria-label="lvm" href="/wsargent/docker-cheat-sheet/commits/master/README.md?author=lvm"><img alt="@lvm" class="avatar" height="20" src="https://avatars2.githubusercontent.com/u/34095?v=3&amp;s=40" width="20" /> </a>

    <button type="button" data-facebox="#blob_contributors_box" class="btn-link others-text">and others</button>

    </div>

    <div id="blob_contributors_box" style="display:none">
      <h2 class="facebox-header" data-facebox-id="facebox-header">Users who have contributed to this file</h2>
      <ul class="facebox-user-list" data-facebox-id="facebox-description">
          <li class="facebox-user-list-item">
            <img alt="@wsargent" height="24" src="https://avatars0.githubusercontent.com/u/71236?v=3&amp;s=48" width="24" />
            <a href="/wsargent">wsargent</a>
          </li>
          <li class="facebox-user-list-item">
            <img alt="@amirbawab" height="24" src="https://avatars1.githubusercontent.com/u/6259858?v=3&amp;s=48" width="24" />
            <a href="/amirbawab">amirbawab</a>
          </li>
          <li class="facebox-user-list-item">
            <img alt="@jalateras" height="24" src="https://avatars3.githubusercontent.com/u/1454089?v=3&amp;s=48" width="24" />
            <a href="/jalateras">jalateras</a>
          </li>
          <li class="facebox-user-list-item">
            <img alt="@ReadmeCritic" height="24" src="https://avatars2.githubusercontent.com/u/15367484?v=3&amp;s=48" width="24" />
            <a href="/ReadmeCritic">ReadmeCritic</a>
          </li>
          <li class="facebox-user-list-item">
            <img alt="@outcoldman" height="24" src="https://avatars0.githubusercontent.com/u/597158?v=3&amp;s=48" width="24" />
            <a href="/outcoldman">outcoldman</a>
          </li>
          <li class="facebox-user-list-item">
            <img alt="@dkhamsing" height="24" src="https://avatars0.githubusercontent.com/u/4723115?v=3&amp;s=48" width="24" />
            <a href="/dkhamsing">dkhamsing</a>
          </li>
          <li class="facebox-user-list-item">
            <img alt="@tuksik" height="24" src="https://avatars1.githubusercontent.com/u/386140?v=3&amp;s=48" width="24" />
            <a href="/tuksik">tuksik</a>
          </li>
          <li class="facebox-user-list-item">
            <img alt="@ttres" height="24" src="https://avatars3.githubusercontent.com/u/493551?v=3&amp;s=48" width="24" />
            <a href="/ttres">ttres</a>
          </li>
          <li class="facebox-user-list-item">
            <img alt="@thorstenc" height="24" src="https://avatars1.githubusercontent.com/u/869096?v=3&amp;s=48" width="24" />
            <a href="/thorstenc">thorstenc</a>
          </li>
          <li class="facebox-user-list-item">
            <img alt="@vdemario" height="24" src="https://avatars3.githubusercontent.com/u/6087424?v=3&amp;s=48" width="24" />
            <a href="/vdemario">vdemario</a>
          </li>
          <li class="facebox-user-list-item">
            <img alt="@lherrera" height="24" src="https://avatars3.githubusercontent.com/u/2963309?v=3&amp;s=48" width="24" />
            <a href="/lherrera">lherrera</a>
          </li>
          <li class="facebox-user-list-item">
            <img alt="@manycoding" height="24" src="https://avatars0.githubusercontent.com/u/10396557?v=3&amp;s=48" width="24" />
            <a href="/manycoding">manycoding</a>
          </li>
          <li class="facebox-user-list-item">
            <img alt="@mariorez" height="24" src="https://avatars0.githubusercontent.com/u/197228?v=3&amp;s=48" width="24" />
            <a href="/mariorez">mariorez</a>
          </li>
          <li class="facebox-user-list-item">
            <img alt="@kxxoling" height="24" src="https://avatars0.githubusercontent.com/u/1227139?v=3&amp;s=48" width="24" />
            <a href="/kxxoling">kxxoling</a>
          </li>
          <li class="facebox-user-list-item">
            <img alt="@rmetzler" height="24" src="https://avatars1.githubusercontent.com/u/58824?v=3&amp;s=48" width="24" />
            <a href="/rmetzler">rmetzler</a>
          </li>
          <li class="facebox-user-list-item">
            <img alt="@PetrGlad" height="24" src="https://avatars2.githubusercontent.com/u/124476?v=3&amp;s=48" width="24" />
            <a href="/PetrGlad">PetrGlad</a>
          </li>
          <li class="facebox-user-list-item">
            <img alt="@ming13" height="24" src="https://avatars2.githubusercontent.com/u/200401?v=3&amp;s=48" width="24" />
            <a href="/ming13">ming13</a>
          </li>
          <li class="facebox-user-list-item">
            <img alt="@vorburger" height="24" src="https://avatars3.githubusercontent.com/u/298598?v=3&amp;s=48" width="24" />
            <a href="/vorburger">vorburger</a>
          </li>
          <li class="facebox-user-list-item">
            <img alt="@kherrick" height="24" src="https://avatars0.githubusercontent.com/u/3065761?v=3&amp;s=48" width="24" />
            <a href="/kherrick">kherrick</a>
          </li>
          <li class="facebox-user-list-item">
            <img alt="@berekuk" height="24" src="https://avatars1.githubusercontent.com/u/89368?v=3&amp;s=48" width="24" />
            <a href="/berekuk">berekuk</a>
          </li>
          <li class="facebox-user-list-item">
            <img alt="@mattreyuk" height="24" src="https://avatars2.githubusercontent.com/u/926405?v=3&amp;s=48" width="24" />
            <a href="/mattreyuk">mattreyuk</a>
          </li>
          <li class="facebox-user-list-item">
            <img alt="@Secathor" height="24" src="https://avatars3.githubusercontent.com/u/107411?v=3&amp;s=48" width="24" />
            <a href="/Secathor">Secathor</a>
          </li>
          <li class="facebox-user-list-item">
            <img alt="@Skamander" height="24" src="https://avatars3.githubusercontent.com/u/4005707?v=3&amp;s=48" width="24" />
            <a href="/Skamander">Skamander</a>
          </li>
          <li class="facebox-user-list-item">
            <img alt="@cschneider4711" height="24" src="https://avatars3.githubusercontent.com/u/6897328?v=3&amp;s=48" width="24" />
            <a href="/cschneider4711">cschneider4711</a>
          </li>
          <li class="facebox-user-list-item">
            <img alt="@LouisVN" height="24" src="https://avatars1.githubusercontent.com/u/18465316?v=3&amp;s=48" width="24" />
            <a href="/LouisVN">LouisVN</a>
          </li>
          <li class="facebox-user-list-item">
            <img alt="@lvm" height="24" src="https://avatars0.githubusercontent.com/u/34095?v=3&amp;s=48" width="24" />
            <a href="/lvm">lvm</a>
          </li>
          <li class="facebox-user-list-item">
            <img alt="@loucal" height="24" src="https://avatars3.githubusercontent.com/u/1024946?v=3&amp;s=48" width="24" />
            <a href="/loucal">loucal</a>
          </li>
          <li class="facebox-user-list-item">
            <img alt="@spacewander" height="24" src="https://avatars1.githubusercontent.com/u/4161644?v=3&amp;s=48" width="24" />
            <a href="/spacewander">spacewander</a>
          </li>
          <li class="facebox-user-list-item">
            <img alt="@lruslan" height="24" src="https://avatars1.githubusercontent.com/u/1275141?v=3&amp;s=48" width="24" />
            <a href="/lruslan">lruslan</a>
          </li>
          <li class="facebox-user-list-item">
            <img alt="@int32bit" height="24" src="https://avatars2.githubusercontent.com/u/5260798?v=3&amp;s=48" width="24" />
            <a href="/int32bit">int32bit</a>
          </li>
          <li class="facebox-user-list-item">
            <img alt="@klingtnet" height="24" src="https://avatars2.githubusercontent.com/u/1538057?v=3&amp;s=48" width="24" />
            <a href="/klingtnet">klingtnet</a>
          </li>
          <li class="facebox-user-list-item">
            <img alt="@jw3" height="24" src="https://avatars1.githubusercontent.com/u/1545372?v=3&amp;s=48" width="24" />
            <a href="/jw3">jw3</a>
          </li>
          <li class="facebox-user-list-item">
            <img alt="@jviide" height="24" src="https://avatars2.githubusercontent.com/u/19776768?v=3&amp;s=48" width="24" />
            <a href="/jviide">jviide</a>
          </li>
          <li class="facebox-user-list-item">
            <img alt="@suchkultur" height="24" src="https://avatars3.githubusercontent.com/u/803252?v=3&amp;s=48" width="24" />
            <a href="/suchkultur">suchkultur</a>
          </li>
          <li class="facebox-user-list-item">
            <img alt="@allingeek" height="24" src="https://avatars1.githubusercontent.com/u/1166083?v=3&amp;s=48" width="24" />
            <a href="/allingeek">allingeek</a>
          </li>
          <li class="facebox-user-list-item">
            <img alt="@jamesvl" height="24" src="https://avatars3.githubusercontent.com/u/354570?v=3&amp;s=48" width="24" />
            <a href="/jamesvl">jamesvl</a>
          </li>
          <li class="facebox-user-list-item">
            <img alt="@wedow" height="24" src="https://avatars1.githubusercontent.com/u/2073046?v=3&amp;s=48" width="24" />
            <a href="/wedow">wedow</a>
          </li>
          <li class="facebox-user-list-item">
            <img alt="@jghaines" height="24" src="https://avatars2.githubusercontent.com/u/977737?v=3&amp;s=48" width="24" />
            <a href="/jghaines">jghaines</a>
          </li>
          <li class="facebox-user-list-item">
            <img alt="@h4cc" height="24" src="https://avatars2.githubusercontent.com/u/2981491?v=3&amp;s=48" width="24" />
            <a href="/h4cc">h4cc</a>
          </li>
          <li class="facebox-user-list-item">
            <img alt="@plainspooky" height="24" src="https://avatars0.githubusercontent.com/u/6437167?v=3&amp;s=48" width="24" />
            <a href="/plainspooky">plainspooky</a>
          </li>
          <li class="facebox-user-list-item">
            <img alt="@geminiyellow" height="24" src="https://avatars1.githubusercontent.com/u/929878?v=3&amp;s=48" width="24" />
            <a href="/geminiyellow">geminiyellow</a>
          </li>
          <li class="facebox-user-list-item">
            <img alt="@FredrikWendt" height="24" src="https://avatars0.githubusercontent.com/u/89504?v=3&amp;s=48" width="24" />
            <a href="/FredrikWendt">FredrikWendt</a>
          </li>
          <li class="facebox-user-list-item">
            <img alt="@thomasleveil" height="24" src="https://avatars0.githubusercontent.com/u/42300?v=3&amp;s=48" width="24" />
            <a href="/thomasleveil">thomasleveil</a>
          </li>
          <li class="facebox-user-list-item">
            <img alt="@tortxof" height="24" src="https://avatars0.githubusercontent.com/u/3578949?v=3&amp;s=48" width="24" />
            <a href="/tortxof">tortxof</a>
          </li>
          <li class="facebox-user-list-item">
            <img alt="@ddysher" height="24" src="https://avatars2.githubusercontent.com/u/2191361?v=3&amp;s=48" width="24" />
            <a href="/ddysher">ddysher</a>
          </li>
          <li class="facebox-user-list-item">
            <img alt="@trenton42" height="24" src="https://avatars0.githubusercontent.com/u/1412655?v=3&amp;s=48" width="24" />
            <a href="/trenton42">trenton42</a>
          </li>
          <li class="facebox-user-list-item">
            <img alt="@dklotz" height="24" src="https://avatars1.githubusercontent.com/u/2143593?v=3&amp;s=48" width="24" />
            <a href="/dklotz">dklotz</a>
          </li>
          <li class="facebox-user-list-item">
            <img alt="@nelsonjchen" height="24" src="https://avatars2.githubusercontent.com/u/5363?v=3&amp;s=48" width="24" />
            <a href="/nelsonjchen">nelsonjchen</a>
          </li>
          <li class="facebox-user-list-item">
            <img alt="@cpjk" height="24" src="https://avatars1.githubusercontent.com/u/3213506?v=3&amp;s=48" width="24" />
            <a href="/cpjk">cpjk</a>
          </li>
          <li class="facebox-user-list-item">
            <img alt="@chaserelock" height="24" src="https://avatars0.githubusercontent.com/u/5704766?v=3&amp;s=48" width="24" />
            <a href="/chaserelock">chaserelock</a>
          </li>
          <li class="facebox-user-list-item">
            <img alt="@bwhaley" height="24" src="https://avatars2.githubusercontent.com/u/503816?v=3&amp;s=48" width="24" />
            <a href="/bwhaley">bwhaley</a>
          </li>
          <li class="facebox-user-list-item">
            <img alt="@blaggacao" height="24" src="https://avatars3.githubusercontent.com/u/7548295?v=3&amp;s=48" width="24" />
            <a href="/blaggacao">blaggacao</a>
          </li>
          <li class="facebox-user-list-item">
            <img alt="@asancheza" height="24" src="https://avatars0.githubusercontent.com/u/2805062?v=3&amp;s=48" width="24" />
            <a href="/asancheza">asancheza</a>
          </li>
          <li class="facebox-user-list-item">
            <img alt="@afolarin" height="24" src="https://avatars2.githubusercontent.com/u/2489685?v=3&amp;s=48" width="24" />
            <a href="/afolarin">afolarin</a>
          </li>
          <li class="facebox-user-list-item">
            <img alt="@yachi" height="24" src="https://avatars2.githubusercontent.com/u/216480?v=3&amp;s=48" width="24" />
            <a href="/yachi">yachi</a>
          </li>
          <li class="facebox-user-list-item">
            <img alt="@marvell" height="24" src="https://avatars1.githubusercontent.com/u/234081?v=3&amp;s=48" width="24" />
            <a href="/marvell">marvell</a>
          </li>
          <li class="facebox-user-list-item">
            <img alt="@annafw" height="24" src="https://avatars2.githubusercontent.com/u/3526523?v=3&amp;s=48" width="24" />
            <a href="/annafw">annafw</a>
          </li>
          <li class="facebox-user-list-item">
            <img alt="@abdul" height="24" src="https://avatars3.githubusercontent.com/u/64568?v=3&amp;s=48" width="24" />
            <a href="/abdul">abdul</a>
          </li>
      </ul>
    </div>
  </div>

<div class="file">
  <div class="file-header">
  <div class="file-actions">

    <div class="BtnGroup">
      <a href="/wsargent/docker-cheat-sheet/raw/master/README.md" class="btn btn-sm BtnGroup-item" id="raw-url">Raw</a>
        <a href="/wsargent/docker-cheat-sheet/blame/master/README.md" class="btn btn-sm js-update-url-with-hash BtnGroup-item">Blame</a>
      <a href="/wsargent/docker-cheat-sheet/commits/master/README.md" class="btn btn-sm BtnGroup-item" rel="nofollow">History</a>
    </div>

        <a class="btn-octicon tooltipped tooltipped-nw"
           href="https://windows.github.com"
           aria-label="Open this file in GitHub Desktop"
           data-ga-click="Repository, open with desktop, type:windows">
            <svg aria-hidden="true" class="octicon octicon-device-desktop" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M15 2H1c-.55 0-1 .45-1 1v9c0 .55.45 1 1 1h5.34c-.25.61-.86 1.39-2.34 2h8c-1.48-.61-2.09-1.39-2.34-2H15c.55 0 1-.45 1-1V3c0-.55-.45-1-1-1zm0 9H1V3h14v8z"/></svg>
        </a>

        <button type="button" class="btn-octicon disabled tooltipped tooltipped-nw"
          aria-label="You must be signed in to make or propose changes">
          <svg aria-hidden="true" class="octicon octicon-pencil" height="16" version="1.1" viewBox="0 0 14 16" width="14"><path fill-rule="evenodd" d="M0 12v3h3l8-8-3-3-8 8zm3 2H1v-2h1v1h1v1zm10.3-9.3L12 6 9 3l1.3-1.3a.996.996 0 0 1 1.41 0l1.59 1.59c.39.39.39 1.02 0 1.41z"/></svg>
        </button>
        <button type="button" class="btn-octicon btn-octicon-danger disabled tooltipped tooltipped-nw"
          aria-label="You must be signed in to make or propose changes">
          <svg aria-hidden="true" class="octicon octicon-trashcan" height="16" version="1.1" viewBox="0 0 12 16" width="12"><path fill-rule="evenodd" d="M11 2H9c0-.55-.45-1-1-1H5c-.55 0-1 .45-1 1H2c-.55 0-1 .45-1 1v1c0 .55.45 1 1 1v9c0 .55.45 1 1 1h7c.55 0 1-.45 1-1V5c.55 0 1-.45 1-1V3c0-.55-.45-1-1-1zm-1 12H3V5h1v8h1V5h1v8h1V5h1v8h1V5h1v9zm1-10H2V3h9v1z"/></svg>
        </button>
  </div>

  <div class="file-info">
      737 lines (477 sloc)
      <span class="file-info-divider"></span>
    35.2 KB
  </div>
</div>

  
  <div id="readme" class="readme blob instapaper_body">
    <article class="markdown-body entry-content" itemprop="text"><h1><a id="user-content-docker-cheat-sheet" class="anchor" href="#docker-cheat-sheet" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Docker Cheat Sheet</h1>

<p><strong>Want to improve this cheat sheet?  See the <a href="#contributing">Contributing</a> section!</strong></p>

<h2><a id="user-content-a-tasteful-plug-for-lightbend" class="anchor" href="#a-tasteful-plug-for-lightbend" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>A Tasteful Plug for Lightbend</h2>

<p>I work for <a href="https://lightbend.com">Lightbend</a> on the <a href="https://playframework.com/">Play</a> team.  I think the company is awesome, and if you're looking at containers because you're moving to the cloud and thinking about distributed systems, you should keep reading.</p>

<p>Lightbend make microservices happen.  Developers use <a href="http://www.lagomframework.com/">Lagom</a> to put together resilient ("chaos monkey resistant") microservices.  In production, there's <a href="https://conductr.lightbend.com/">Conductr</a> to <a href="http://www.cakesolutions.net/teamblogs/typesafe-conductr-the-missing-glue-between-dev-and-ops">orchestrate</a> containers -- <a href="https://www.lightbend.com/blog/reactive-for-devops-part-3-using-docker-with-conductr-on-the-jvm">including Docker</a>.  Finally, there's <a href="https://developer.lightbend.com/docs/monitoring/latest/home.html">monitoring</a> to tell you what's going on at a detailed application level, so you know where your CPU and memory resources are being spent, and can scale up and down based on that information.  For more, check out the <a href="https://www.lightbend.com/platform/production">devops site</a>.</p>

<p>This concludes the tasteful plug.</p>

<h2><a id="user-content-table-of-contents" class="anchor" href="#table-of-contents" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Table of Contents</h2>

<ul>
<li><a href="#why-docker">Why Docker</a></li>
<li><a href="#prerequisites">Prerequisites</a></li>
<li><a href="#installation">Installation</a></li>
<li><a href="#containers">Containers</a></li>
<li><a href="#images">Images</a></li>
<li><a href="#networks">Networks</a></li>
<li><a href="#registry--repository">Registry and Repository</a></li>
<li><a href="#dockerfile">Dockerfile</a></li>
<li><a href="#layers">Layers</a></li>
<li><a href="#links">Links</a></li>
<li><a href="#volumes">Volumes</a></li>
<li><a href="#exposing-ports">Exposing Ports</a></li>
<li><a href="#best-practices">Best Practices</a></li>
<li><a href="#security">Security</a></li>
<li><a href="#tips">Tips</a></li>
<li><a href="#contributing">Contributing</a></li>
</ul>

<h2><a id="user-content-why-docker" class="anchor" href="#why-docker" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Why Docker</h2>

<p>"With Docker, developers can build any app in any language using any toolchain. “Dockerized” apps are completely portable and can run anywhere - colleagues’ OS X and Windows laptops, QA servers running Ubuntu in the cloud, and production data center VMs running Red Hat.</p>

<p>Developers can get going quickly by starting with one of the 13,000+ apps available on Docker Hub. Docker manages and tracks changes and dependencies, making it easier for sysadmins to understand how the apps that developers build work. And with Docker Hub, developers can automate their build pipeline and share artifacts with collaborators through public or private repositories.</p>

<p>Docker helps developers build and ship higher-quality applications, faster." -- <a href="https://www.docker.com/what-docker#copy1">What is Docker</a></p>

<h2><a id="user-content-prerequisites" class="anchor" href="#prerequisites" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Prerequisites</h2>

<p>I use <a href="https://github.com/robbyrussell/oh-my-zsh">Oh My Zsh</a> with the <a href="https://github.com/robbyrussell/oh-my-zsh/wiki/Plugins#docker">Docker plugin</a> for autocompletion of docker commands. YMMV.</p>

<h3><a id="user-content-linux" class="anchor" href="#linux" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Linux</h3>

<p>The 3.10.x kernel is <a href="https://docs.docker.com/engine/installation/binaries/#check-kernel-dependencies">the minimum requirement</a> for Docker.</p>

<h3><a id="user-content-macos" class="anchor" href="#macos" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>MacOS</h3>

<p>10.8 “Mountain Lion” or newer is required.</p>

<h2><a id="user-content-installation" class="anchor" href="#installation" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Installation</h2>

<h3><a id="user-content-linux-1" class="anchor" href="#linux-1" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Linux</h3>

<p>Quick and easy install script provided by Docker:</p>

<pre><code>curl -sSL https://get.docker.com/ | sh
</code></pre>

<p>If you're not willing to run a random shell script, please see the <a href="https://docs.docker.com/engine/installation/linux/">installation</a> instructions for your distribution.</p>

<p>If you are a complete Docker newbie, you should follow the <a href="https://docs.docker.com/engine/getstarted/">series of tutorials</a> now.</p>

<h3><a id="user-content-mac-os-x" class="anchor" href="#mac-os-x" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Mac OS X</h3>

<p>Download and install <a href="https://docs.docker.com/toolbox/overview/">Docker Toolbox</a>.  <a href="https://docs.docker.com/docker-for-mac/">Docker For Mac</a> is nice, but it's not quite as finished as the VirtualBox install.  <a href="https://docs.docker.com/docker-for-mac/docker-toolbox/">See the comparison</a>.</p>

<blockquote>
<p><strong>NOTE</strong> If you have an existing docker toolbox, you might think you can upgrade <a href="https://docs.docker.com/machine/install-machine/">Docker Machine</a> binaries directly (either from URL or <code>docker-machine upgrade default</code>) and it will take care of itself.  This is not going to help -- <code>docker-machine</code> will be <code>1.10.3</code> while <code>docker</code> is still <code>1.8.3</code> or whatever your previous version is.</p>

<p>You are much better off using Docker Toolbox DMG file to upgrade, which will take care of all the binaries at once.</p>
</blockquote>

<p>Once you've installed Docker Toolbox, install a VM with Docker Machine using the VirtualBox provider:</p>

<pre><code>docker-machine create --driver=virtualbox default
docker-machine ls
eval "$(docker-machine env default)"
</code></pre>

<p>Then start up a container:</p>

<pre><code>docker run hello-world
</code></pre>

<p>That's it, you have a running Docker container.</p>

<p>If you are a complete Docker newbie, you should probably follow the <a href="https://docs.docker.com/engine/getstarted/">series of tutorials</a> now.</p>

<h2><a id="user-content-containers" class="anchor" href="#containers" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Containers</h2>

<p><a href="http://etherealmind.com/basics-docker-containers-hypervisors-coreos/">Your basic isolated Docker process</a>. Containers are to Virtual Machines as threads are to processes. Or you can think of them as chroots on steroids.</p>

<h3><a id="user-content-lifecycle" class="anchor" href="#lifecycle" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Lifecycle</h3>

<ul>
<li><a href="https://docs.docker.com/engine/reference/commandline/create"><code>docker create</code></a> creates a container but does not start it.</li>
<li><a href="https://docs.docker.com/engine/reference/commandline/rename/"><code>docker rename</code></a> allows the container to be renamed.</li>
<li><a href="https://docs.docker.com/engine/reference/commandline/run"><code>docker run</code></a> creates and starts a container in one operation.</li>
<li><a href="https://docs.docker.com/engine/reference/commandline/rm"><code>docker rm</code></a> deletes a container.</li>
<li><a href="https://docs.docker.com/engine/reference/commandline/update/"><code>docker update</code></a> updates a container's resource limits.</li>
</ul>

<p>If you want a transient container, <code>docker run --rm</code> will remove the container after it stops.</p>

<p>If you want to map a directory on the host to a docker container, <code>docker run -v $HOSTDIR:$DOCKERDIR</code>. Also see <a href="https://github.com/wsargent/docker-cheat-sheet/#volumes">Volumes</a>.</p>

<p>If you want to remove also the volumes associated with the container, the deletion of the container must include the <code>-v</code> switch like in <code>docker rm -v</code>.</p>

<p>There's also a <a href="https://docs.docker.com/engine/admin/logging/overview/">logging driver</a> available for individual containers in docker 1.10. To run docker with a custom log driver (i.e., to syslog), use <code>docker run --log-driver=syslog</code>.</p>

<h3><a id="user-content-starting-and-stopping" class="anchor" href="#starting-and-stopping" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Starting and Stopping</h3>

<ul>
<li><a href="https://docs.docker.com/engine/reference/commandline/start"><code>docker start</code></a> starts a container so it is running.</li>
<li><a href="https://docs.docker.com/engine/reference/commandline/stop"><code>docker stop</code></a> stops a running container.</li>
<li><a href="https://docs.docker.com/engine/reference/commandline/restart"><code>docker restart</code></a> stops and starts a container.</li>
<li><a href="https://docs.docker.com/engine/reference/commandline/pause/"><code>docker pause</code></a> pauses a running container, "freezing" it in place.</li>
<li><a href="https://docs.docker.com/engine/reference/commandline/unpause/"><code>docker unpause</code></a> will unpause a running container.</li>
<li><a href="https://docs.docker.com/engine/reference/commandline/wait"><code>docker wait</code></a> blocks until running container stops.</li>
<li><a href="https://docs.docker.com/engine/reference/commandline/kill"><code>docker kill</code></a> sends a SIGKILL to a running container.</li>
<li><a href="https://docs.docker.com/engine/reference/commandline/attach"><code>docker attach</code></a> will connect to a running container.</li>
</ul>

<p>If you want to integrate a container with a <a href="https://docs.docker.com/engine/admin/host_integration/">host process manager</a>, start the daemon with <code>-r=false</code> then use <code>docker start -a</code>.</p>

<p>If you want to expose container ports through the host, see the <a href="#exposing-ports">exposing ports</a> section.</p>

<p>Restart policies on crashed docker instances are <a href="http://container42.com/2014/09/30/docker-restart-policies/">covered here</a>.</p>

<h4><a id="user-content-cpu-constraints" class="anchor" href="#cpu-constraints" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>CPU Constraints</h4>

<p>You can limit CPU, either using a percentage of all CPUs, or by using specific cores.  </p>

<p>For example, you can tell the <a href="https://docs.docker.com/engine/reference/run/#/cpu-share-constraint"><code>cpu-shares</code></a> setting.  The setting is a bit strange -- 1024 means 100% of the CPU, so if you want the container to take 50% of all CPU cores, you should specify 512.  See <a href="https://goldmann.pl/blog/2014/09/11/resource-management-in-docker/#_cpu">https://goldmann.pl/blog/2014/09/11/resource-management-in-docker/#_cpu</a> for more:</p>

<pre><code>docker run -ti --c 512 agileek/cpuset-test
</code></pre>

<p>You can also only use some CPU cores using <a href="https://docs.docker.com/engine/reference/run/#/cpuset-constraint"><code>cpuset-cpus</code></a>.  See <a href="https://agileek.github.io/docker/2014/08/06/docker-cpuset/">https://agileek.github.io/docker/2014/08/06/docker-cpuset/</a> for details and some nice videos:</p>

<pre><code>docker run -ti --cpuset-cpus=0,4,6 agileek/cpuset-test
</code></pre>

<p>Note that Docker can still <strong>see</strong> all of the CPUs inside the container -- it just isn't using all of them.  See <a href="https://github.com/docker/docker/issues/20770">https://github.com/docker/docker/issues/20770</a> for more details.</p>

<h4><a id="user-content-memory-constraints" class="anchor" href="#memory-constraints" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Memory Constraints</h4>

<p>You can also set <a href="https://docs.docker.com/engine/reference/run/#/user-memory-constraints">memory constraints</a> on Docker:</p>

<pre><code>docker run -it -m 300M ubuntu:14.04 /bin/bash
</code></pre>

<h4><a id="user-content-capabilities" class="anchor" href="#capabilities" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Capabilities</h4>

<p>Linux capabilities can be set by using <code>cap-add</code> and <code>cap-drop</code>.  See <a href="https://docs.docker.com/engine/reference/run/#/runtime-privilege-and-linux-capabilities">https://docs.docker.com/engine/reference/run/#/runtime-privilege-and-linux-capabilities</a> for details.  This should be used for greater security.</p>

<p>To mount a FUSE based filesystem, you need to combine both --cap-add and --device:</p>

<pre><code>docker run --rm -it --cap-add SYS_ADMIN --device /dev/fuse sshfs
</code></pre>

<p>Give access to a single device:</p>

<pre><code>docker run -it --device=/dev/ttyUSB0 debian bash
</code></pre>

<p>Give access to all devices:</p>

<pre><code>docker run -it --privileged -v /dev/bus/usb:/dev/bus/usb debian bash
</code></pre>

<p>more info about privileged containers <a href="https://docs.docker.com/engine/reference/run/#/runtime-privilege-and-linux-capabilities">here</a></p>

<h3><a id="user-content-info" class="anchor" href="#info" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Info</h3>

<ul>
<li><a href="https://docs.docker.com/engine/reference/commandline/ps"><code>docker ps</code></a> shows running containers.</li>
<li><a href="https://docs.docker.com/engine/reference/commandline/logs"><code>docker logs</code></a> gets logs from container.  (You can use a custom log driver, but logs is only available for <code>json-file</code> and <code>journald</code> in 1.10).</li>
<li><a href="https://docs.docker.com/engine/reference/commandline/inspect"><code>docker inspect</code></a> looks at all the info on a container (including IP address).</li>
<li><a href="https://docs.docker.com/engine/reference/commandline/events"><code>docker events</code></a> gets events from container.</li>
<li><a href="https://docs.docker.com/engine/reference/commandline/port"><code>docker port</code></a> shows public facing port of container.</li>
<li><a href="https://docs.docker.com/engine/reference/commandline/top"><code>docker top</code></a> shows running processes in container.</li>
<li><a href="https://docs.docker.com/engine/reference/commandline/stats"><code>docker stats</code></a> shows containers' resource usage statistics.</li>
<li><a href="https://docs.docker.com/engine/reference/commandline/diff"><code>docker diff</code></a> shows changed files in the container's FS.</li>
</ul>

<p><code>docker ps -a</code> shows running and stopped containers.</p>

<p><code>docker stats --all</code> shows a running list of containers.</p>

<h3><a id="user-content-import--export" class="anchor" href="#import--export" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Import / Export</h3>

<ul>
<li><a href="https://docs.docker.com/engine/reference/commandline/cp"><code>docker cp</code></a> copies files or folders between a container and the local filesystem.</li>
<li><a href="https://docs.docker.com/engine/reference/commandline/export"><code>docker export</code></a> turns container filesystem into tarball archive stream to STDOUT.</li>
</ul>

<h3><a id="user-content-executing-commands" class="anchor" href="#executing-commands" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Executing Commands</h3>

<ul>
<li><a href="https://docs.docker.com/engine/reference/commandline/exec"><code>docker exec</code></a> to execute a command in container.</li>
</ul>

<p>To enter a running container, attach a new shell process to a running container called foo, use: <code>docker exec -it foo /bin/bash</code>.</p>

<h2><a id="user-content-images" class="anchor" href="#images" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Images</h2>

<p>Images are just <a href="https://docs.docker.com/engine/understanding-docker/#how-does-a-docker-image-work">templates for docker containers</a>.</p>

<h3><a id="user-content-lifecycle-1" class="anchor" href="#lifecycle-1" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Lifecycle</h3>

<ul>
<li><a href="https://docs.docker.com/engine/reference/commandline/images"><code>docker images</code></a> shows all images.</li>
<li><a href="https://docs.docker.com/engine/reference/commandline/import"><code>docker import</code></a> creates an image from a tarball.</li>
<li><a href="https://docs.docker.com/engine/reference/commandline/build"><code>docker build</code></a> creates image from Dockerfile.</li>
<li><a href="https://docs.docker.com/engine/reference/commandline/commit"><code>docker commit</code></a> creates image from a container, pausing it temporarily if it is running.</li>
<li><a href="https://docs.docker.com/engine/reference/commandline/rmi"><code>docker rmi</code></a> removes an image.</li>
<li><a href="https://docs.docker.com/engine/reference/commandline/load"><code>docker load</code></a> loads an image from a tar archive as STDIN, including images and tags (as of 0.7).</li>
<li><a href="https://docs.docker.com/engine/reference/commandline/save"><code>docker save</code></a> saves an image to a tar archive stream to STDOUT with all parent layers, tags &amp; versions (as of 0.7).</li>
</ul>

<h3><a id="user-content-info-1" class="anchor" href="#info-1" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Info</h3>

<ul>
<li><a href="https://docs.docker.com/engine/reference/commandline/history"><code>docker history</code></a> shows history of image.</li>
<li><a href="https://docs.docker.com/engine/reference/commandline/tag"><code>docker tag</code></a> tags an image to a name (local or registry).</li>
</ul>

<h3><a id="user-content-cleaning-up" class="anchor" href="#cleaning-up" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Cleaning up</h3>

<p>While you can use the <code>docker rmi</code> command to remove specific images, there's a tool called <a href="https://github.com/spotify/docker-gc">docker-gc</a> that will clean up images that are no longer used by any containers in a safe manner.</p>

<h3><a id="user-content-loadsave-image" class="anchor" href="#loadsave-image" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Load/Save image</h3>

<p>Load an image from file:</p>

<pre><code>docker load &lt; my_image.tar.gz
</code></pre>

<p>Save an existing image:</p>

<pre><code>docker save my_image:my_tag &gt; my_image.tar.gz
</code></pre>

<h3><a id="user-content-importexport-container" class="anchor" href="#importexport-container" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Import/Export container</h3>

<p>Import a container as an image from file:</p>

<pre><code>cat my_container.tar.gz | docker import - my_image:my_tag
</code></pre>

<p>Export an existing container:</p>

<pre><code>docker export my_container &gt; my_container.tar.gz
</code></pre>

<h3><a id="user-content-difference-between-loading-a-saved-image-and-importing-an-exported-container-as-an-image-" class="anchor" href="#difference-between-loading-a-saved-image-and-importing-an-exported-container-as-an-image-" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Difference between loading a saved image and importing an exported container as an image ?</h3>

<p>Loading an image using the <code>load</code> command creates a new image including its history.<br>
Importing a container as an image using the <code>import</code> command creates a new image excluding the history which results in a smaller image size compared to loading an image.</p>

<h2><a id="user-content-networks" class="anchor" href="#networks" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Networks</h2>

<p>Docker has a <a href="https://docs.docker.com/engine/userguide/networking/">networks</a> feature. Not much is known about it, so this is a good place to expand the cheat sheet. There is a note saying that it's a good way to configure docker containers to talk to each other without using ports. See <a href="https://docs.docker.com/engine/userguide/networking/work-with-networks/">working with networks</a> for more details.</p>

<h3><a id="user-content-lifecycle-2" class="anchor" href="#lifecycle-2" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Lifecycle</h3>

<ul>
<li><a href="https://docs.docker.com/engine/reference/commandline/network_create/"><code>docker network create</code></a></li>
<li><a href="https://docs.docker.com/engine/reference/commandline/network_rm/"><code>docker network rm</code></a></li>
</ul>

<h3><a id="user-content-info-2" class="anchor" href="#info-2" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Info</h3>

<ul>
<li><a href="https://docs.docker.com/engine/reference/commandline/network_ls/"><code>docker network ls</code></a></li>
<li><a href="https://docs.docker.com/engine/reference/commandline/network_inspect/"><code>docker network inspect</code></a></li>
</ul>

<h3><a id="user-content-connection" class="anchor" href="#connection" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Connection</h3>

<ul>
<li><a href="https://docs.docker.com/engine/reference/commandline/network_connect/"><code>docker network connect</code></a></li>
<li><a href="https://docs.docker.com/engine/reference/commandline/network_disconnect/"><code>docker network disconnect</code></a></li>
</ul>

<p>You can specify a <a href="https://blog.jessfraz.com/post/ips-for-all-the-things/">specific IP address for a container</a>:</p>

<pre><code># create a new bridge network with your subnet and gateway for your ip block
docker network create --subnet 203.0.113.0/24 --gateway 203.0.113.254 iptastic

# run a nginx container with a specific ip in that block
$ docker run --rm -it --net iptastic --ip 203.0.113.2 nginx

# curl the ip from any other place (assuming this is a public ip block duh)
$ curl 203.0.113.2
</code></pre>

<h2><a id="user-content-registry--repository" class="anchor" href="#registry--repository" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Registry &amp; Repository</h2>

<p>A repository is a <em>hosted</em> collection of tagged images that together create the file system for a container.</p>

<p>A registry is a <em>host</em> -- a server that stores repositories and provides an HTTP API for <a href="https://docs.docker.com/engine/tutorials/dockerrepos/">managing the uploading and downloading of repositories</a>.</p>

<p>Docker.com hosts its own <a href="https://hub.docker.com/">index</a> to a central registry which contains a large number of repositories.  Having said that, the central docker registry <a href="https://titanous.com/posts/docker-insecurity">does not do a good job of verifying images</a> and should be avoided if you're worried about security.</p>

<ul>
<li><a href="https://docs.docker.com/engine/reference/commandline/login"><code>docker login</code></a> to login to a registry.</li>
<li><a href="https://docs.docker.com/engine/reference/commandline/logout"><code>docker logout</code></a> to logout from a registry.</li>
<li><a href="https://docs.docker.com/engine/reference/commandline/search"><code>docker search</code></a> searches registry for image.</li>
<li><a href="https://docs.docker.com/engine/reference/commandline/pull"><code>docker pull</code></a> pulls an image from registry to local machine.</li>
<li><a href="https://docs.docker.com/engine/reference/commandline/push"><code>docker push</code></a> pushes an image to the registry from local machine.</li>
</ul>

<h3><a id="user-content-run-local-registry" class="anchor" href="#run-local-registry" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Run local registry</h3>

<p>You can run a local registry by using the <a href="https://github.com/docker/distribution">docker distribution</a> project and looking at the <a href="https://github.com/docker/docker.github.io/blob/master/registry/deploying.md">local deploy</a> instructions.</p>

<p>Also see the <a href="https://groups.google.com/a/dockerproject.org/forum/#!forum/distribution">mailing list</a>.</p>

<h2><a id="user-content-dockerfile" class="anchor" href="#dockerfile" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Dockerfile</h2>

<p><a href="https://docs.docker.com/engine/reference/builder/">The configuration file</a>. Sets up a Docker container when you run <code>docker build</code> on it. Vastly preferable to <code>docker commit</code>.  </p>

<p>Here are some common text editors and their syntax highlighting modules you could use to create Dockerfiles:</p>

<ul>
<li>If you use <a href="http://jedit.org">jEdit</a>, I've put up a syntax highlighting module for <a href="https://github.com/wsargent/jedit-docker-mode">Dockerfile</a> you can use.</li>
<li><a href="https://packagecontrol.io/packages/Dockerfile%20Syntax%20Highlighting">Sublime Text 2</a></li>
<li><a href="https://atom.io/packages/language-docker">Atom</a></li>
<li><a href="https://github.com/ekalinin/Dockerfile.vim">Vim</a></li>
<li><a href="https://github.com/spotify/dockerfile-mode">Emacs</a></li>
<li><a href="https://github.com/docker/docker/tree/master/contrib/syntax/textmate">TextMate</a></li>
<li>For a most comprehensive list of editors and IDEs, check <a href="https://domeide.github.io/">Docker meets the IDE</a></li>
</ul>

<h3><a id="user-content-instructions" class="anchor" href="#instructions" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Instructions</h3>

<ul>
<li><a href="https://docs.docker.com/engine/reference/builder/#dockerignore-file">.dockerignore</a></li>
<li><a href="https://docs.docker.com/engine/reference/builder/#from">FROM</a> Sets the Base Image for subsequent instructions.</li>
<li><a href="https://docs.docker.com/engine/reference/builder/#maintainer">MAINTAINER</a> Set the Author field of the generated images..</li>
<li><a href="https://docs.docker.com/engine/reference/builder/#run">RUN</a> execute any commands in a new layer on top of the current image and commit the results.</li>
<li><a href="https://docs.docker.com/engine/reference/builder/#cmd">CMD</a> provide defaults for an executing container.</li>
<li><a href="https://docs.docker.com/engine/reference/builder/#expose">EXPOSE</a> informs Docker that the container listens on the specified network ports at runtime.  NOTE: does not actually make ports accessible.</li>
<li><a href="https://docs.docker.com/engine/reference/builder/#env">ENV</a> sets environment variable.</li>
<li><a href="https://docs.docker.com/engine/reference/builder/#add">ADD</a> copies new files, directories or remote file to container.  Invalidates caches. Avoid <code>ADD</code> and use <code>COPY</code> instead.</li>
<li><a href="https://docs.docker.com/engine/reference/builder/#copy">COPY</a> copies new files or directories to container.</li>
<li><a href="https://docs.docker.com/engine/reference/builder/#entrypoint">ENTRYPOINT</a> configures a container that will run as an executable.</li>
<li><a href="https://docs.docker.com/engine/reference/builder/#volume">VOLUME</a> creates a mount point for externally mounted volumes or other containers.</li>
<li><a href="https://docs.docker.com/engine/reference/builder/#user">USER</a> sets the user name for following RUN / CMD / ENTRYPOINT commands.</li>
<li><a href="https://docs.docker.com/engine/reference/builder/#workdir">WORKDIR</a> sets the working directory.</li>
<li><a href="https://docs.docker.com/engine/reference/builder/#arg">ARG</a> defines a build-time variable.</li>
<li><a href="https://docs.docker.com/engine/reference/builder/#onbuild">ONBUILD</a> adds a trigger instruction when the image is used as the base for another build.</li>
<li><a href="https://docs.docker.com/engine/reference/builder/#stopsignal">STOPSIGNAL</a> sets the system call signal that will be sent to the container to exit.</li>
<li><a href="https://docs.docker.com/engine/userguide/labels-custom-metadata/">LABEL</a> apply key/value metadata to your images, containers, or daemons.</li>
</ul>

<h3><a id="user-content-tutorial" class="anchor" href="#tutorial" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Tutorial</h3>

<ul>
<li><a href="http://flux7.com/blogs/docker/docker-tutorial-series-part-3-automation-is-the-word-using-dockerfile/">Flux7's Dockerfile Tutorial</a></li>
</ul>

<h3><a id="user-content-examples" class="anchor" href="#examples" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Examples</h3>

<ul>
<li><a href="https://docs.docker.com/engine/reference/builder/#dockerfile-examples">Examples</a></li>
<li><a href="https://docs.docker.com/engine/userguide/eng-image/dockerfile_best-practices/">Best practices for writing Dockerfiles</a></li>
<li><a href="http://crosbymichael.com/">Michael Crosby</a> has some more <a href="http://crosbymichael.com/dockerfile-best-practices.html">Dockerfiles best practices</a> / <a href="http://crosbymichael.com/dockerfile-best-practices-take-2.html">take 2</a>.</li>
<li><a href="http://jonathan.bergknoff.com/journal/building-good-docker-images">Building Good Docker Images</a> / <a href="http://jonathan.bergknoff.com/journal/building-better-docker-images">Building Better Docker Images</a></li>
<li><a href="https://speakerdeck.com/garethr/managing-container-configuration-with-metadata">Managing Container Configuration with Metadata</a></li>
</ul>

<h2><a id="user-content-layers" class="anchor" href="#layers" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Layers</h2>

<p>The versioned filesystem in Docker is based on layers. They're like <a href="https://docs.docker.com/engine/userguide/storagedriver/imagesandcontainers/">git commits or changesets for filesystems</a>.</p>

<p>Note that if you're using <a href="https://en.wikipedia.org/wiki/Aufs">aufs</a> as your filesystem, Docker does not always remove data volumes containers layers when you delete a container! See <a href="https://github.com/docker/docker/pull/8484">PR 8484</a> for more details.</p>

<h2><a id="user-content-links" class="anchor" href="#links" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Links</h2>

<p>Links are how Docker containers talk to each other <a href="https://docs.docker.com/engine/userguide/networking/default_network/dockerlinks/">through TCP/IP ports</a>. <a href="https://docs.docker.com/engine/examples/running_redis_service/">Linking into Redis</a> and <a href="https://blogs.atlassian.com/2013/11/docker-all-the-things-at-atlassian-automation-and-wiring/">Atlassian</a> show worked examples. You can also resolve <a href="https://docs.docker.com/engine/userguide/networking/default_network/dockerlinks/#/updating-the-etchosts-file">links by hostname</a>.</p>

<p>NOTE: If you want containers to ONLY communicate with each other through links, start the docker daemon with <code>-icc=false</code> to disable inter process communication.</p>

<p>If you have a container with the name CONTAINER (specified by <code>docker run --name CONTAINER</code>) and in the Dockerfile, it has an exposed port:</p>

<pre><code>EXPOSE 1337
</code></pre>

<p>Then if we create another container called LINKED like so:</p>

<pre><code>docker run -d --link CONTAINER:ALIAS --name LINKED user/wordpress
</code></pre>

<p>Then the exposed ports and aliases of CONTAINER will show up in LINKED with the following environment variables:</p>

<pre><code>$ALIAS_PORT_1337_TCP_PORT
$ALIAS_PORT_1337_TCP_ADDR
</code></pre>

<p>And you can connect to it that way.</p>

<p>To delete links, use <code>docker rm --link</code>.</p>

<p>Generally, linking between docker services is a subset of "service discovery", a big problem if you're planning to use Docker at scale in production.  Please read <a href="https://www.digitalocean.com/community/tutorials/the-docker-ecosystem-service-discovery-and-distributed-configuration-stores">The Docker Ecosystem: Service Discovery and Distributed Configuration Stores</a> for more info.</p>

<h2><a id="user-content-volumes" class="anchor" href="#volumes" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Volumes</h2>

<p>Docker volumes are <a href="https://docs.docker.com/engine/tutorials/dockervolumes/">free-floating filesystems</a>. They don't have to be connected to a particular container. You should use volumes mounted from <a href="https://medium.com/@ramangupta/why-docker-data-containers-are-good-589b3c6c749e">data-only containers</a> for portability.  </p>

<h3><a id="user-content-lifecycle-3" class="anchor" href="#lifecycle-3" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Lifecycle</h3>

<ul>
<li><a href="https://docs.docker.com/engine/reference/commandline/volume_create/"><code>docker volume create</code></a></li>
<li><a href="https://docs.docker.com/engine/reference/commandline/volume_rm/"><code>docker volume rm</code></a></li>
</ul>

<h3><a id="user-content-info-3" class="anchor" href="#info-3" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Info</h3>

<ul>
<li><a href="https://docs.docker.com/engine/reference/commandline/volume_ls/"><code>docker volume ls</code></a></li>
<li><a href="https://docs.docker.com/engine/reference/commandline/volume_inspect/"><code>docker volume inspect</code></a></li>
</ul>

<p>Volumes are useful in situations where you can't use links (which are TCP/IP only). For instance, if you need to have two docker instances communicate by leaving stuff on the filesystem.</p>

<p>You can mount them in several docker containers at once, using <code>docker run --volumes-from</code>.</p>

<p>Because volumes are isolated filesystems, they are often used to store state from computations between transient containers. That is, you can have a stateless and transient container run from a recipe, blow it away, and then have a second instance of the transient container pick up from where the last one left off.</p>

<p>See <a href="http://crosbymichael.com/advanced-docker-volumes.html">advanced volumes</a> for more details. Container42 is <a href="http://container42.com/2014/11/03/docker-indepth-volumes/">also helpful</a>.</p>

<p>You can <a href="https://docs.docker.com/engine/tutorials/dockervolumes/#mount-a-host-directory-as-a-data-volume">map MacOS host directories as docker volumes</a>:</p>

<pre><code>docker run -v /Users/wsargent/myapp/src:/src
</code></pre>

<p>You can use remote NFS volumes if you're <a href="https://docs.docker.com/engine/tutorials/dockervolumes/#/mount-a-shared-storage-volume-as-a-data-volume">feeling brave</a>.</p>

<p>You may also consider running data-only containers as described <a href="http://container42.com/2013/12/16/persistent-volumes-with-docker-container-as-volume-pattern/">here</a> to provide some data portability.</p>

<h2><a id="user-content-exposing-ports" class="anchor" href="#exposing-ports" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Exposing ports</h2>

<p>Exposing incoming ports through the host container is <a href="https://docs.docker.com/engine/reference/run/#expose-incoming-ports">fiddly but doable</a>.</p>

<p>This is done by mapping the container port to the host port (only using localhost interface) using <code>-p</code>:</p>

<pre><code>docker run -p 127.0.0.1:$HOSTPORT:$CONTAINERPORT --name CONTAINER -t someimage
</code></pre>

<p>You can tell Docker that the container listens on the specified network ports at runtime by using <a href="https://docs.docker.com/engine/reference/builder/#expose">EXPOSE</a>:</p>

<pre><code>EXPOSE &lt;CONTAINERPORT&gt;
</code></pre>

<p>Note that EXPOSE does not expose the port itself -- only <code>-p</code> will do that. To expose the container's port on your localhost's port:</p>

<pre><code>iptables -t nat -A DOCKER -p tcp --dport &lt;LOCALHOSTPORT&gt; -j DNAT --to-destination &lt;CONTAINERIP&gt;:&lt;PORT&gt;
</code></pre>

<p>If you're running Docker in Virtualbox, you then need to forward the port there as well, using <a href="https://docs.vagrantup.com/v2/networking/forwarded_ports.html">forwarded_port</a>. Define a range of ports in your Vagrantfile like this so you can dynamically map them:</p>

<pre><code>Vagrant.configure(VAGRANTFILE_API_VERSION) do |config|
  ...

  (49000..49900).each do |port|
    config.vm.network :forwarded_port, :host =&gt; port, :guest =&gt; port
  end

  ...
end
</code></pre>

<p>If you forget what you mapped the port to on the host container, use <code>docker port</code> to show it:</p>

<pre><code>docker port CONTAINER $CONTAINERPORT
</code></pre>

<h2><a id="user-content-best-practices" class="anchor" href="#best-practices" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Best Practices</h2>

<p>This is where general Docker best practices and war stories go:</p>

<ul>
<li><a href="http://gregoryszorc.com/blog/2014/10/16/the-rabbit-hole-of-using-docker-in-automated-tests/">The Rabbit Hole of Using Docker in Automated Tests</a></li>
<li><a href="https://twitter.com/bridgetkromhout">Bridget Kromhout</a> has a useful blog post on <a href="http://sysadvent.blogspot.co.uk/2014/12/day-1-docker-in-production-reality-not.html">running Docker in production</a> at Dramafever.</li>
<li>There's also a best practices <a href="http://developers.lyst.com/devops/2014/12/08/docker/">blog post</a> from Lyst.</li>
<li><a href="https://engineering.salesforceiq.com/2013/11/05/a-docker-dev-environment-in-24-hours-part-2-of-2.html">A Docker Dev Environment in 24 Hours!</a></li>
<li><a href="https://tersesystems.com/2013/11/20/building-a-development-environment-with-docker/">Building a Development Environment With Docker</a></li>
<li><a href="https://samsaffron.com/archive/2013/11/07/discourse-in-a-docker-container">Discourse in a Docker Container</a></li>
</ul>

<h2><a id="user-content-security" class="anchor" href="#security" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Security</h2>

<p>This is where security tips about Docker go. The Docker <a href="https://docs.docker.com/engine/security/security/">security</a> page goes into more detail.</p>

<p>First things first: Docker runs as root. If you are in the <code>docker</code> group, you effectively <a href="http://reventlov.com/advisories/using-the-docker-command-to-root-the-host">have root access</a>. If you expose the docker unix socket to a container, you are giving the container <a href="https://www.lvh.io/posts/dont-expose-the-docker-socket-not-even-to-a-container.html">root access to the host</a>.  </p>

<p>Docker should not be your only defense. You should secure and harden it.</p>

<p>For an understanding of what containers leave exposed, you should read is <a href="https://www.nccgroup.trust/globalassets/our-research/us/whitepapers/2016/april/ncc_group_understanding_hardening_linux_containers-10pdf">Understanding and Hardening Linux Containers</a> by <a href="https://twitter.com/dyn___">Aaron Grattafiori</a>. This is a complete and comprehensive guide to the issues involved with containers, with a plethora of links and footnotes leading on to yet more useful content. The security tips following are useful if you've already hardened containers in the past, but are not a substitute for understanding.</p>

<h3><a id="user-content-security-tips" class="anchor" href="#security-tips" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Security Tips</h3>

<p>For greatest security, you want to run Docker inside a virtual machine. This is straight from the Docker Security Team Lead -- <a href="http://www.slideshare.net/jpetazzo/linux-containers-lxc-docker-and-security">slides</a> / <a href="http://www.projectatomic.io/blog/2014/08/is-it-safe-a-look-at-docker-and-security-from-linuxcon/">notes</a>. Then, run with AppArmor / seccomp / SELinux / grsec etc to <a href="http://linux-audit.com/docker-security-best-practices-for-your-vessel-and-containers/">limit the container permissions</a>. See the <a href="https://blog.docker.com/2016/02/docker-engine-1-10-security/">Docker 1.10 security features</a> for more details.</p>

<p>Docker image ids are <a href="https://medium.com/@quayio/your-docker-image-ids-are-secrets-and-its-time-you-treated-them-that-way-f55e9f14c1a4">sensitive information</a> and should not be exposed to the outside world. Treat them like passwords.</p>

<p>See the <a href="https://github.com/konstruktoid/Docker/blob/master/Security/CheatSheet.adoc">Docker Security Cheat Sheet</a> by <a href="https://github.com/konstruktoid">Thomas Sjögren</a>: some good stuff about container hardening in there.</p>

<p>Check out the <a href="https://github.com/docker/docker-bench-security">docker bench security script</a>, download the <a href="https://blog.docker.com/2015/05/understanding-docker-security-and-best-practices/">white papers</a> and subscribe to the <a href="https://www.docker.com/docker-security">mailing lists</a> (unfortunately Docker does not have a unique mailing list, only dev / user).</p>

<p>You should start off by using a kernel with unstable patches for grsecurity / pax compiled in, such as <a href="https://en.wikipedia.org/wiki/Alpine_Linux">Alpine Linux</a>. If you are using grsecurity in production, you should spring for <a href="https://grsecurity.net/business_support.php">commercial support</a> for the <a href="https://grsecurity.net/announce.php">stable patches</a>, same as you would do for RedHat. It's $200 a month, which is nothing to your devops budget.</p>

<p>Since docker 1.11 you can easily limit the number of active processes running inside a container to prevent fork bombs. This requires a linux kernel &gt;= 4.3 with CGROUP_PIDS=y to be in the kernel configuration.</p>

<pre><code>docker run --pids-limit=64
</code></pre>

<p>Also available since docker 1.11 is the ability to prevent processes from gaining new privileges. This feature have been in the linux kernel since version 3.5. You can read more about it in <a href="http://www.projectatomic.io/blog/2016/03/no-new-privs-docker/">this</a> blog post.</p>

<pre><code>docker run --security-opt=no-new-privileges
</code></pre>

<p>From the <a href="http://container-solutions.com/content/uploads/2015/06/15.06.15_DockerCheatSheet_A2.pdf">Docker Security Cheat Sheet</a> (it's in PDF which makes it hard to use, so copying below) by <a href="http://container-solutions.com/is-docker-safe-for-production/">Container Solutions</a>:</p>

<p>Turn off interprocess communication with:</p>

<pre><code>docker -d --icc=false --iptables
</code></pre>

<p>Set the container to be read-only:</p>

<pre><code>docker run --read-only
</code></pre>

<p>Verify images with a hashsum:</p>

<pre><code>docker pull debian@sha256:a25306f3850e1bd44541976aa7b5fd0a29be
</code></pre>

<p>Set volumes to be read only:</p>

<pre><code>docker run -v $(pwd)/secrets:/secrets:ro debian
</code></pre>

<p>Define and run a user in your Dockerfile so you don't run as root inside the container:</p>

<pre><code>RUN groupadd -r user &amp;&amp; useradd -r -g user user
USER user
</code></pre>

<h3><a id="user-content-user-namespaces" class="anchor" href="#user-namespaces" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>User Namespaces</h3>

<p>There's also work on <a href="https://s3hh.wordpress.com/2013/07/19/creating-and-using-containers-without-privilege/">user namespaces</a> -- it is in 1.10 but is not enabled by default.</p>

<p>To enable user namespaces ("remap the userns") in Ubuntu 15.10, <a href="https://raesene.github.io/blog/2016/02/04/Docker-User-Namespaces/">follow the blog example</a>.</p>

<h3><a id="user-content-security-videos" class="anchor" href="#security-videos" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Security Videos</h3>

<ul>
<li><a href="https://youtu.be/04LOuMgNj9U">Using Docker Safely</a></li>
<li><a href="https://youtu.be/KmxOXmPhZbk">Securing your applications using Docker</a></li>
<li><a href="https://youtu.be/a9lE9Urr6AQ">Container security: Do containers actually contain?</a></li>
<li><a href="https://www.youtube.com/watch?v=iN6QbszB1R8">Linux Containers: Future or Fantasy?</a></li>
</ul>

<h3><a id="user-content-security-roadmap" class="anchor" href="#security-roadmap" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Security Roadmap</h3>

<p>The Docker roadmap talks about <a href="https://github.com/docker/docker/blob/master/ROADMAP.md#11-security">seccomp support</a>.
There is an AppArmor policy generator called <a href="https://github.com/jfrazelle/bane">bane</a>, and they're working on <a href="https://github.com/docker/docker/issues/17142">security profiles</a>.</p>

<h2><a id="user-content-tips" class="anchor" href="#tips" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Tips</h2>

<p>Sources:</p>

<ul>
<li><a href="http://sssslide.com/speakerdeck.com/bmorearty/15-docker-tips-in-5-minutes">15 Docker Tips in 5 minutes</a></li>
</ul>

<h3><a id="user-content-last-ids" class="anchor" href="#last-ids" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Last Ids</h3>

<pre><code>alias dl='docker ps -l -q'
docker run ubuntu echo hello world
docker commit $(dl) helloworld
</code></pre>

<h3><a id="user-content-commit-with-command-needs-dockerfile" class="anchor" href="#commit-with-command-needs-dockerfile" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Commit with command (needs Dockerfile)</h3>

<pre><code>docker commit -run='{"Cmd":["postgres", "-too -many -opts"]}' $(dl) postgres
</code></pre>

<h3><a id="user-content-get-ip-address" class="anchor" href="#get-ip-address" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Get IP address</h3>

<pre><code>docker inspect $(dl) | grep IPAddress | cut -d '"' -f 4
</code></pre>

<p>or install <a href="https://stedolan.github.io/jq/">jq</a>:</p>

<pre><code>docker inspect $(dl) | jq -r '.[0].NetworkSettings.IPAddress'
</code></pre>

<p>or using a <a href="https://docs.docker.com/engine/reference/commandline/inspect">go template</a>:</p>

<pre><code>docker inspect -f '{{ .NetworkSettings.IPAddress }}' &lt;container_name&gt;
</code></pre>

<h3><a id="user-content-get-port-mapping" class="anchor" href="#get-port-mapping" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Get port mapping</h3>

<pre><code>docker inspect -f '{{range $p, $conf := .NetworkSettings.Ports}} {{$p}} -&gt; {{(index $conf 0).HostPort}} {{end}}' &lt;containername&gt;
</code></pre>

<h3><a id="user-content-find-containers-by-regular-expression" class="anchor" href="#find-containers-by-regular-expression" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Find containers by regular expression</h3>

<pre><code>for i in $(docker ps -a | grep "REGEXP_PATTERN" | cut -f1 -d" "); do echo $i; done
</code></pre>

<h3><a id="user-content-get-environment-settings" class="anchor" href="#get-environment-settings" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Get Environment Settings</h3>

<pre><code>docker run --rm ubuntu env
</code></pre>

<h3><a id="user-content-kill-running-containers" class="anchor" href="#kill-running-containers" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Kill running containers</h3>

<pre><code>docker kill $(docker ps -q)
</code></pre>

<h3><a id="user-content-delete-old-containers" class="anchor" href="#delete-old-containers" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Delete old containers</h3>

<pre><code>docker ps -a | grep 'weeks ago' | awk '{print $1}' | xargs docker rm
</code></pre>

<h3><a id="user-content-delete-stopped-containers" class="anchor" href="#delete-stopped-containers" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Delete stopped containers</h3>

<pre><code>docker rm -v $(docker ps -a -q -f status=exited)
</code></pre>

<h3><a id="user-content-delete-dangling-images" class="anchor" href="#delete-dangling-images" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Delete dangling images</h3>

<pre><code>docker rmi $(docker images -q -f dangling=true)
</code></pre>

<h3><a id="user-content-delete-all-images" class="anchor" href="#delete-all-images" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Delete all images</h3>

<pre><code>docker rmi $(docker images -q)
</code></pre>

<h3><a id="user-content-delete-dangling-volumes" class="anchor" href="#delete-dangling-volumes" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Delete dangling volumes</h3>

<p>As of Docker 1.9:</p>

<pre><code>docker volume rm $(docker volume ls -q -f dangling=true)
</code></pre>

<p>In 1.9.0, the filter <code>dangling=false</code> does <em>not</em> work - it is ignored and will list all volumes.</p>

<h3><a id="user-content-show-image-dependencies" class="anchor" href="#show-image-dependencies" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Show image dependencies</h3>

<pre><code>docker images -viz | dot -Tpng -o docker.png
</code></pre>

<h3><a id="user-content-slimming-down-docker-containers-see-intercity-blog" class="anchor" href="#slimming-down-docker-containers-see-intercity-blog" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Slimming down Docker containers (see <a href="http://bit.ly/1Wwo61N">Intercity Blog</a>)</h3>

<ul>
<li>Cleaning APT in a RUN layer</li>
</ul>

<p>This should be done in the same layer as other apt commands.
Otherwise, the previous layers still persist the original information and your images will still be fat.</p>

<pre><code>RUN {apt commands} \
 &amp;&amp; apt-get clean \
 &amp;&amp; rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
</code></pre>

<ul>
<li>Flatten an image</li>
</ul>

<pre><code>ID=$(docker run -d image-name /bin/bash)
docker export $ID | docker import – flat-image-name
</code></pre>

<ul>
<li>For backup</li>
</ul>

<pre><code>ID=$(docker run -d image-name /bin/bash)
(docker export $ID | gzip -c &gt; image.tgz)
gzip -dc image.tgz | docker import - flat-image-name
</code></pre>

<h3><a id="user-content-monitor-system-resource-utilization-for-running-containers" class="anchor" href="#monitor-system-resource-utilization-for-running-containers" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Monitor system resource utilization for running containers</h3>

<p>To check the CPU, memory, and network I/O usage of a single container, you can use:</p>

<pre><code>docker stats &lt;container&gt;
</code></pre>

<p>For all containers listed by id:</p>

<pre><code>docker stats $(docker ps -q)
</code></pre>

<p>For all containers listed by name:</p>

<pre><code>docker stats $(docker ps --format '{{.Names}}')
</code></pre>

<p>For all containers listed by image:</p>

<pre><code>docker ps -a -f ancestor=ubuntu
</code></pre>

<h2><a id="user-content-contributing" class="anchor" href="#contributing" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Contributing</h2>

<p>Here's how to contribute to this cheat sheet.</p>

<h3><a id="user-content-open-readmemd" class="anchor" href="#open-readmemd" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Open README.md</h3>

<p>Click <a href="https://github.com/wsargent/docker-cheat-sheet/blob/master/README.md">README.md</a> &lt;-- this link</p>

<p><a href="/wsargent/docker-cheat-sheet/blob/master/images/click.png" target="_blank"><img src="/wsargent/docker-cheat-sheet/raw/master/images/click.png" alt="Click This" style="max-width:100%;"></a></p>

<h3><a id="user-content-edit-page" class="anchor" href="#edit-page" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Edit Page</h3>

<p><a href="/wsargent/docker-cheat-sheet/blob/master/images/edit.png" target="_blank"><img src="/wsargent/docker-cheat-sheet/raw/master/images/edit.png" alt="Edit This" style="max-width:100%;"></a></p>

<h3><a id="user-content-make-changes-and-commit" class="anchor" href="#make-changes-and-commit" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Make Changes and Commit</h3>

<p><a href="/wsargent/docker-cheat-sheet/blob/master/images/change.png" target="_blank"><img src="/wsargent/docker-cheat-sheet/raw/master/images/change.png" alt="Change This" style="max-width:100%;"></a></p>

<p><a href="/wsargent/docker-cheat-sheet/blob/master/images/commit.png" target="_blank"><img src="/wsargent/docker-cheat-sheet/raw/master/images/commit.png" alt="Commit" style="max-width:100%;"></a></p>
</article>
  </div>

</div>

<button type="button" data-facebox="#jump-to-line" data-facebox-class="linejump" data-hotkey="l" class="d-none">Jump to Line</button>
<div id="jump-to-line" style="display:none">
  <!-- '"` --><!-- </textarea></xmp> --></option></form><form accept-charset="UTF-8" action="" class="js-jump-to-line-form" method="get"><div style="margin:0;padding:0;display:inline"><input name="utf8" type="hidden" value="&#x2713;" /></div>
    <input class="form-control linejump-input js-jump-to-line-field" type="text" placeholder="Jump to line&hellip;" aria-label="Jump to line" autofocus>
    <button type="submit" class="btn">Go</button>
</form></div>

  </div>
  <div class="modal-backdrop js-touch-events"></div>
</div>


    </div>
  </div>

    </div>

        <div class="container site-footer-container">
  <div class="site-footer" role="contentinfo">
    <ul class="site-footer-links float-right">
        <li><a href="https://github.com/contact" data-ga-click="Footer, go to contact, text:contact">Contact GitHub</a></li>
      <li><a href="https://developer.github.com" data-ga-click="Footer, go to api, text:api">API</a></li>
      <li><a href="https://training.github.com" data-ga-click="Footer, go to training, text:training">Training</a></li>
      <li><a href="https://shop.github.com" data-ga-click="Footer, go to shop, text:shop">Shop</a></li>
        <li><a href="https://github.com/blog" data-ga-click="Footer, go to blog, text:blog">Blog</a></li>
        <li><a href="https://github.com/about" data-ga-click="Footer, go to about, text:about">About</a></li>

    </ul>

    <a href="https://github.com" aria-label="Homepage" class="site-footer-mark" title="GitHub">
      <svg aria-hidden="true" class="octicon octicon-mark-github" height="24" version="1.1" viewBox="0 0 16 16" width="24"><path fill-rule="evenodd" d="M8 0C3.58 0 0 3.58 0 8c0 3.54 2.29 6.53 5.47 7.59.4.07.55-.17.55-.38 0-.19-.01-.82-.01-1.49-2.01.37-2.53-.49-2.69-.94-.09-.23-.48-.94-.82-1.13-.28-.15-.68-.52-.01-.53.63-.01 1.08.58 1.23.82.72 1.21 1.87.87 2.33.66.07-.52.28-.87.51-1.07-1.78-.2-3.64-.89-3.64-3.95 0-.87.31-1.59.82-2.15-.08-.2-.36-1.02.08-2.12 0 0 .67-.21 2.2.82.64-.18 1.32-.27 2-.27.68 0 1.36.09 2 .27 1.53-1.04 2.2-.82 2.2-.82.44 1.1.16 1.92.08 2.12.51.56.82 1.27.82 2.15 0 3.07-1.87 3.75-3.65 3.95.29.25.54.73.54 1.48 0 1.07-.01 1.93-.01 2.2 0 .21.15.46.55.38A8.013 8.013 0 0 0 16 8c0-4.42-3.58-8-8-8z"/></svg>
</a>
    <ul class="site-footer-links">
      <li>&copy; 2016 <span title="0.06089s from github-fe141-cp1-prd.iad.github.net">GitHub</span>, Inc.</li>
        <li><a href="https://github.com/site/terms" data-ga-click="Footer, go to terms, text:terms">Terms</a></li>
        <li><a href="https://github.com/site/privacy" data-ga-click="Footer, go to privacy, text:privacy">Privacy</a></li>
        <li><a href="https://github.com/security" data-ga-click="Footer, go to security, text:security">Security</a></li>
        <li><a href="https://status.github.com/" data-ga-click="Footer, go to status, text:status">Status</a></li>
        <li><a href="https://help.github.com" data-ga-click="Footer, go to help, text:help">Help</a></li>
    </ul>
  </div>
</div>



    

    <div id="ajax-error-message" class="ajax-error-message flash flash-error">
      <svg aria-hidden="true" class="octicon octicon-alert" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M8.865 1.52c-.18-.31-.51-.5-.87-.5s-.69.19-.87.5L.275 13.5c-.18.31-.18.69 0 1 .19.31.52.5.87.5h13.7c.36 0 .69-.19.86-.5.17-.31.18-.69.01-1L8.865 1.52zM8.995 13h-2v-2h2v2zm0-3h-2V6h2v4z"/></svg>
      <button type="button" class="flash-close js-flash-close js-ajax-error-dismiss" aria-label="Dismiss error">
        <svg aria-hidden="true" class="octicon octicon-x" height="16" version="1.1" viewBox="0 0 12 16" width="12"><path fill-rule="evenodd" d="M7.48 8l3.75 3.75-1.48 1.48L6 9.48l-3.75 3.75-1.48-1.48L4.52 8 .77 4.25l1.48-1.48L6 6.52l3.75-3.75 1.48 1.48z"/></svg>
      </button>
      You can't perform that action at this time.
    </div>


      
      <script crossorigin="anonymous" integrity="sha256-LkSqcbUyVnVb/pNN00YzECBYVDe2mFf3k8aPbA39LP4=" src="https://assets-cdn.github.com/assets/frameworks-2e44aa71b53256755bfe934dd346331020585437b69857f793c68f6c0dfd2cfe.js"></script>
      <script async="async" crossorigin="anonymous" integrity="sha256-8OipRQnXQsCOpDT1ySuGzwu6D6slsZtBu8UL36KDZVQ=" src="https://assets-cdn.github.com/assets/github-f0e8a94509d742c08ea434f5c92b86cf0bba0fab25b19b41bbc50bdfa2836554.js"></script>
      
      
      
      
    <div class="js-stale-session-flash stale-session-flash flash flash-warn flash-banner d-none">
      <svg aria-hidden="true" class="octicon octicon-alert" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M8.865 1.52c-.18-.31-.51-.5-.87-.5s-.69.19-.87.5L.275 13.5c-.18.31-.18.69 0 1 .19.31.52.5.87.5h13.7c.36 0 .69-.19.86-.5.17-.31.18-.69.01-1L8.865 1.52zM8.995 13h-2v-2h2v2zm0-3h-2V6h2v4z"/></svg>
      <span class="signed-in-tab-flash">You signed in with another tab or window. <a href="">Reload</a> to refresh your session.</span>
      <span class="signed-out-tab-flash">You signed out in another tab or window. <a href="">Reload</a> to refresh your session.</span>
    </div>
    <div class="facebox" id="facebox" style="display:none;">
  <div class="facebox-popup">
    <div class="facebox-content" role="dialog" aria-labelledby="facebox-header" aria-describedby="facebox-description">
    </div>
    <button type="button" class="facebox-close js-facebox-close" aria-label="Close modal">
      <svg aria-hidden="true" class="octicon octicon-x" height="16" version="1.1" viewBox="0 0 12 16" width="12"><path fill-rule="evenodd" d="M7.48 8l3.75 3.75-1.48 1.48L6 9.48l-3.75 3.75-1.48-1.48L4.52 8 .77 4.25l1.48-1.48L6 6.52l3.75-3.75 1.48 1.48z"/></svg>
    </button>
  </div>
</div>

  </body>
</html>


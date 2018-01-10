---
layout: post
title: ActiveRecord Bypass in Rails
---

```
Every craftsman starts his or her journey with a basic set of good-quality tools.
```

ActiveRecord is such a tool. 

It is the object relational mapper (ORM) used in Rails. It's extremely convenient as it performs validations on models, provides a consistent interface to your data store, etc.. Given this usefulness though, there are situations where the interface it provides isn't sufficient to perform a particular action. It's a tool, as are the programming languages we choose, the editors we grow fond of (vim > emacs), and the practices we subscribe to. As a software engineer with the aspiration of pragmatism, the tools we choose to use depend upon the problem we're solving.

This article will cover the situation where you find yourself writing raw SQL in a Rails project, using the native driver of your data store. I'll cover PostgreSQL for the sake of simplicity (and because that's what I faced), but the ideas should translate relatively well.

Note: I'm skipping over any installation or setup of the data store, for brevity sake.

### Connecting to your native driver

<script src="https://gist.github.com/brandon-powers/974730be59d46bd98926e906fcef58e6.js"></script>

If you happen to disagree with any of the points in this article, or want to express your comments, feel free to contact me through the "About" section on this site.

Thank you for reading, I hope you found this article useful and/or interesting. 

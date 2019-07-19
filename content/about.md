---
title: "About"
date: 2019-07-14T19:14:50+02:00
author: "Ulisse Mini"
---

## Hi there

<p id="age">My name is Uli and I was born in 2004.</p>
I made it so I could write about the things I learn and hopefully someone else can benifit from it too.

<script>
  "use strict";

  const birth_year = 2004;
  const birth_month = 9;

  const current_month = new Date().getMonth();
  const current_year = new Date().getFullYear();

  let my_age = current_year - birth_year;
  if (current_month < birth_month) {
    my_age--;
  }

  const age = document.getElementById("age");

  age.innerHTML = age.innerHTML.replace("I was born in 2004", "I'm " + my_age + " years old");
</script>

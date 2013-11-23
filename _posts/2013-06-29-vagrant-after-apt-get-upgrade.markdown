---
layout: post
title: "vagrant after apt-get upgrade"
published: true
---

It is the solution I found: https://github.com/mitchellh/vagrant/issues/733

check output of lsmod | grep vboxsf, empty? if yes, need rebuild the guest extentions.

/etc/init.d/vboxadd setup

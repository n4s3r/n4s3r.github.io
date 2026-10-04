---  
title: "Waft"    
date: 2024-04-12
description: "An OSINT investigation of an old bussiness"
tags:
  - osint
  - investigation
  - dns
  - google-dorks
  - archive-org
  - domain-research
  - reconnaissance
  - open-source-intelligence
---  
A few days ago, I was in my home, trying to repair a radiator. And I was inspecting a piece of the radiator that was broken like this:
<img class="img-narrow" src="/images/osint/Waft/waft.jpg" alt="First search">

And in internet doesn't appreared the website of the vendor. So I thought it was a nice opportunity to start an OSINT invesigation easily.

- First of all, I tried to find the website of the vendor, Waft. 
![First search](images/osint/Waft/first_search.jpg)
You can see in the image, in the right, down, there's a website: www.waftcontrol.com.

So I tried to connect to that website, but didn't work:
![Browser connect](images/osint/Waft/browser_dns.jpg)

That didn't work because doesn't exists www.waftcontrol.com:
![DNS](images/osint/Waft/dns.jpg)

So I tried to search more information using google dorks. My idea was gather information about the website when it existed. But didn't work:
![Dorks](images/osint/Waft/dorks.jpg)

I tried to use another dorks like this, but It didn't work:
![Dorks2](images/osint/Waft/dorks2.jpg)

To try to end this, I searched the domain "www.waftcontrol.com" in archive.org. The last copy of the website, was in 2021:
![Archive1](images/osint/Waft/archive1.jpg)

And I could find the copy of the website that I was looking for:
![archive2](images/osint/Waft/archive2.jpg)

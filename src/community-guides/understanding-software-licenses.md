# Understanding Software Licenses

## What is a software license?
A software license is a legal instrument that gives you the right to install, use or otherwise interact with a specific computer program under given circumstances. 

In simple terms, a software license defines a set of responsibilities for those who use the code and those who produce the code.

A software license is a requirement when releasing code to the public, as without one, the code is copyrighted to the developer by default.

## Why are software licenses important?
Here are the reasons why software licenses are indispensable:

- They define the usage rights (T&C) and prevent unauthorized usage of the software.

- Software licenses are essential for establishing legal boundaries and preventing legal troubles such as fines and lawsuits.

- Licenses are crucial for defining distribution permissions and limitations.

- They allow developers to control how their software is used to prevent misuse and unapproved modifications.

- Open-source licenses facilitate collaboration by providing a legal framework for a transparent development environment. 

## What are the types of Software Licenses? 
There are mainly 4 main categories of Software Licenses based on the rights and restrictions they impose.

### 1. Public Domain
Public Domain software refers to software deliberately placed in the public domain, no longer protected by copyright, trademark or patent laws. As a result, it can be freely used without the permission of or payment to the developer. 

Direct licensing for the public domain is not universally recognized. Here are two tools that you could use as alternatives.  

- **Creative Commons Zero (CC0):** CC0, provided by Creative Commons, is used for waving copyright interest in a work you've created and serves as a fallback as a public domain equivalent license.
- **The Unlicense:** The Unlicense is similar to CC0 but offers a simpler, more direct statement of public domain dedication. 

### 2. Permissive 
Permissive licenses, often referred to as “BSD-style licenses”, contain minimal restrictions on how the software can be modified or redistributed. 

[The Open Source Initiative](https://opensource.org/) defines a permissive software license as a “non-copyleft license that guarantees the freedom to use, modify and redistribute”. 

Some commonly used permissive licenses are:

- **MIT License:** The MIT License is one of the most permissive licenses that allow you to use, copy, modify, distribute, sublicense and sell copies of the software as long as you add a copy of the original MIT License and copyright to it. 
- **Apache License 2.0:** Apache License is similar to MIT License but it explicitly addresses patents by providing the recipient with a license to any patents held by the contributor related to the project.
- **BSD License 2.0:** Much like the MIT License, the BSDv2 License also allows you to use, modify, distribute and sublicense the software. However, it includes an additional requirement for attribution in advertising materials.


### 3. Copyleft
Copyleft licenses are more restrictive and less commercial-friendly. 
These require that anyone who modifies or distributes the software share their changes under the same or a compatible license.

Some commonly used copyleft licenses are:

- **GNU General Public License (GPL) 2.0:** To utilise GPLv2 rights (copying, distribution & modifying), you must track changes and dates in the source file and share any changes under GPL terms.
- **GNU General Public License (GPL) 3.0:** GPLv3 follows GPLv2 but also includes provisions for patents, allows adding extra permissions, improved internationalization and termination processes, etc.
- **GNU Affero General Public License (AGPL) 3.0:** AGPLv3 and GPLv3 share core principles of copyleft, but AGPLv3 includes additional provisions to address the distribution of modified software over a network.   

### 4. Proprietary
Also called closed-sourced, this license is used by developers or vendors to claim ownership of their work and software. Proprietary licenses restrict the user’s right to modify, distribute or access the underlying source code of the software.
An example of a proprietary license is:

- **MS Reference Source License:** The MS-RSL is a proprietary license that allows you to review the code and make copies of it, but you can’t use the code or change it in any way. 

## Comparison of Software Licenses
Here’s a table summarizing the software licenses we talked about earlier, including their types, key features and examples of projects corresponding to each license.

| License                  | Type                | Key Features                                               | Example Projects                 |
|--------------------------|---------------------|------------------------------------------------------------|----------------------------------|
| **GNU General Public License (GPL)**    | Copyleft           |  Requires derivative works to be distributed under the GPL. | Linux, Git, GNU tools            |
| **MIT License**           | Permissive         |  Allows almost unrestricted use, modification, and distribution. | Node.js, jQuery, Rails           |
| **Apache License**        | Permissive         |  Allows usage of the software for any purpose, with limited conditions. | Apache HTTP Server, Hadoop       |
| **BSD Licenses**          | Permissive         |  Simple and permissive, allows use in proprietary projects.  | FreeBSD, NetBSD, Nginx            |
| **Creative Commons**      | Various            |  Used for creative works, it provides different levels of sharing and usage permissions. | Wikimedia Commons, Flickr        |
| **Mozilla Public License (MPL)**        | Copyleft           |  Requires modifications to be open-sourced under the MPL.    | Mozilla Firefox, Thunderbird    |
| **Eclipse Public License (EPL)**        | Weak Copyleft      |  Similar to the MPL, but contains specific patent grant provisions. | Eclipse IDE, Jetty               |
| **ISC License**           | Permissive         |  Short and simple permissive license.                        | OpenBSD, PostCSS                 |
| **GNU Lesser General Public License (LGPL)** | Weak Copyleft  |  Allows linking with non-GPL software.                     | GTK+, GStreamer                  |
| **Unlicense**             | Public Domain      |  Places the work in the public domain with no restrictions.  | Bitcoin.php, CPython (prior to v3.5) |

## Which software license should I use? 

When choosing an open-source license for your project, it’s crucial to ensure that your selection aligns with your ideological values and objectives. Additionally, consider the level of control you wish to maintain over your project, ensuring compatibility and compliance with the licenses of any software incorporated into it.

If you prefer a copyleft approach, where derivative work must also be open source, the GNU General Public License (GPL) is a strong candidate. This license ensures that modifications and improvements to your project also contribute to the open-source community. 

If you prioritize making your software widely accessible with minimal restrictions, the MIT License is a popular choice. It allows for almost unrestricted use, modification and distribution.

There are also open-source software licenses for non-software works ranging from documentation to fonts.

Ultimately, the right license depends on your specific project requirements and how you envision collaboration within the open-source community. Take time to understand the terms and conditions of each license to make an informed decision that best suits your objectives.


## Resources
Not sure which license to pick? Here are a few tools to help you out.

- [Choosealicense.com](https://choosealicense.com/) by Github offers comprehensive information on licensing options beyond those discussed here. 
- [Public License Selector](https://ufal.github.io/public-license-selector/) by ÚFAL is a tool that can help you choose the right open-source license for data and software.

---

This wiki is maintained by [u/govind_s_nair](https://www.reddit.com/user/govind_s_nair).

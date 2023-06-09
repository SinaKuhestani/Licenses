# How to Choose a License for Your Own Work

---

People often ask us what license we recommend they use for their project. We've written about this publicly before, but the information has been scattered around between different essays, FAQ entries, and license commentaries. This article collects all that information into a single source, to make it easier for people to follow and refer back to.


These recommendations are for works designed to do practical jobs. Those include software, documentation, and some other things. Works of art, and works that state a point of view, are different issues; the GNU Project has no general stand about how they should be released, except that they should all be usable without nonfree software (in particular, without DRM). However, you might want to follow these recommendations for art works that go with a particular program.


The recommendations apply to licensing a work that you create—whether that's a modification of an existing work, or a new original work. They do not address the issue of combining existing material under different licenses. If you're looking for help with that, please check our GPL FAQ.

After you see what we recommend here, if you'd like advice, you can write to <licensing@gnu.org>. Note that it will probably take a few weeks for the licensing team to get back to you; if you get no response in a month, please write again.


## Contributing to an existing project


When you contribute to an existing project, you should usually release your modified versions under the same license as the original work. It's good to cooperate with the project's maintainers, and using a different license for your modifications often makes that cooperation very difficult. You should only do that when there is a strong reason to justify it.


One case where using a different license can be justified is when you make major changes to a work under a non-copyleft license. If the version you've created is considerably more useful than the original, then it's worth copylefting your work, for all the same reasons we normally recommend copyleft. If you are in this situation, please follow the recommendations below for licensing a new project.


If you choose to release your contributions under a different license for whatever reason, you must make sure that the original license allows use of the material under your chosen license. For honesty's sake, show explicitly which parts of the work are under which license.


### Software


We recommend different licenses for different projects, depending mostly on the software's purpose. In general, we recommend using the strongest copyleft license that doesn't interfere with that purpose. Our essay “What is Copyleft?” explains the concept of copyleft in more detail, and why it is generally the best licensing strategy.


For most programs, we recommend that you use the most recent version of the GNU General Public License (GPL) for your project. Its strong copyleft is appropriate for all kinds of software, and includes numerous protections for users' freedom. To allow for future license upgrades, please specify “version 3 or any later version” so that your program will be license-compatible with code that may be released, in the future, under subsequent GPL versions.


### Small programs


It is not worth the trouble to use copyleft for most small programs. We use 300 lines as our benchmark: when a software package's source code is shorter than that, the benefits provided by copyleft are usually too small to justify the inconvenience of making sure a copy of the license always accompanies the software.


For those programs, we recommend the Apache License 2.0. This is a weak, lax, “pushover” (non-copyleft) software license that has terms to prevent contributors and distributors from suing for patent infringement. This doesn't make the software immune to threats from patents (no software license can achieve that), but it does prevent patent holders from setting up a “bait and switch” where they release the software under free terms then require recipients to agree to nonfree terms in a patent license.


Among the weak (pushover) licenses, Apache 2.0 is best; so if you are going to use a weak license, whatever the reason, we recommend using that one.


###  Libraries


For libraries, we distinguish three kind of cases.


Some libraries implement free data formats that are competing against restricted data formats, such as Ogg Vorbis (which competes against MP3 audio) and WebM (which competes against MPEG-4 video). The success of the free format requires allowing many proprietary application programs to link in the code to handle the format. For instance, we wanted nonfree media players, especially appliances, to include the code for Ogg Vorbis as well as MP3.


In these special situations, if you are aiming to convince proprietary application developers to use the library for the free format, you would need to make that easy by licensing the library under a weak license, such as the Apache License 2.0.


However, we must recognize that this strategy did not succeed for Ogg Vorbis. Even after changing the copyright license to permit easy inclusion of that library code in proprietary applications, proprietary developers generally did not include it. The sacrifice made in the choice of license ultimately won us little.


For all other libraries, we recommend some kind of copyleft. If developers are already using an established alternative library released under a nonfree license or a lax pushover license, then we recommend using the GNU Lesser General Public License (LGPL).


Unlike the first case, where the library implements an ethically superior standard, here adoption for its own sake will not accomplish any special objective goal, so there's no reason to avoid copyleft entirely. However, if you require developers who use your library to release their whole programs under copyleft, they'll simply use one of the alternatives available, and that won't advance our cause either. The Lesser GPL was designed to fill the middle ground between these cases, allowing proprietary software developers to use the covered library, but providing a weak copyleft that gives users freedom regarding the library code itself.


For libraries that provide specialized facilities, and which do not face entrenched noncopylefted or nonfree competition, we recommend using the plain GNU GPL. For the reasons why, read “Why you shouldn't use the Lesser GPL for your next library.”


### Server Software


If it is likely that others will make improved versions of your program to run on servers and not distribute their versions to anyone else, and you're concerned that this will put your released version at a disadvantage, we recommend the GNU Affero General Public License (AGPL). The AGPL's terms are almost identical to the GPL's; the sole substantive difference is that it has an extra condition to ensure that people who use the software over a network will be able to get the source code for it.


The AGPL's requirement doesn't address the problems that can arise for users when they entrust their computing or their data to someone else's server. For instance, it won't stop Service as a Software Substitute (SaaSS) from denying users' freedom—but most servers don't do SaaSS. For more about these issues, read “Why the Affero GPL.”


### Documentation


We recommend the GNU Free Documentation License (GFDL) for tutorials, reference manuals and other large works of documentation. It's a strong copyleft license for educational works, initially written for software manuals, and includes terms which specifically address common issues that arise when those works are distributed or modified.


For short, secondary documentation works, such as a reference card, it is better to use the GNU all-permissive license, since a copy of the GFDL could hardly fit in a reference card. Don't use CC BY, since it is incompatible with the GFDL.


For man pages, we recommend the GFDL if the page is long, and the GNU all-permissive license if it is short.


Some documentation includes software source code. For instance, a manual for a programming language might include examples for readers to follow. You should both include these in the manual under the FDL's terms, and release them under another license that's appropriate for software. Doing so helps make it easy to use the code in other projects. We recommend that you dedicate small pieces of code to the public domain using CC0, and distribute larger pieces under the same license that the associated software project uses.


### Other data for programs


This section discusses all other works for practical use that you might include with software. To give you some examples, this includes icons and other functional or useful graphics, fonts, and geographic data. You can also follow them for art, though we wouldn't criticize if you don't.


If you are creating these works specifically for use with a software project, we generally recommend that you release your work under the same license as the software. There is no problem in doing so with the licenses we have recommended: GPLv3, LGPLv3, AGPLv3, and GPLv2 can all be applied to any kind of work—not just software—that is copyrightable and has a clear preferred form for modification. Using the same license as the software will help make compliance easier for distributors, and avoids any doubt about potential compatibility issues. Using a different free license may be appropriate if it provides some specific practical benefit, like better cooperation with other free projects.


If your work is not being created for use with a particular software project, or if it wouldn't be appropriate to use the same license as the project, then we only recommend that you choose a copyleft license that's appropriate for your work. We have some of these listed on our license list. If no license seems especially appropriate, the Creative Commons Attribution-ShareAlike license is a copyleft that can be used for many different kinds of works.
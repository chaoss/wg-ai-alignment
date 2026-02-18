# AI Aligment - Moderation Resources and Links


## Awesome LLM Policy

Looking to craft an LLM or Generative AI policy for your project?

Look no further than this repo!

We aim to collect together a wide variety of examples of:
- published AI policies from projects or organizations
- examples of the kinds of behavior AI policies are meant to prevent
- Other resources that may be helpful 

### Project AI Policies
* [Python (Devguide)](https://devguide.python.org/getting-started/generative-ai/)
* [Zulip](https://github.com/zulip/zulip/blob/main/CONTRIBUTING.md#ai-use-policy-and-guidelines)
* [Ladybird Browser](https://github.com/LadybirdBrowser/ladybird/blob/master/CONTRIBUTING.md#on-usage-of-ai-and-llms)
* [Python attrs](https://github.com/python-attrs/attrs/commit/6c54145aac47b60a4c0838acead291ae4a298771)
* [Linux Kernel](https://lore.kernel.org/ksummit/20251114183528.1239900-1-dave.hansen@linux.intel.com/)
* [Servo](https://book.servo.org/contributing.html#ai-contributions) ([discussion](https://github.com/servo/servo/discussions/36379))
* [Gentoo](https://wiki.gentoo.org/wiki/Project:Council/AI_policy)
* Kubernetes ([discussion 1](https://github.com/kubernetes/steering/issues/291), [discussion 2](https://github.com/kubernetes/community/issues/8558))
* [Castle Game Engine](https://castle-engine.io/) - [Rules for contributing and using AI](https://castle-engine.io/ai)
* [FastAPI](https://fastapi.tiangolo.com/contributing/#automated-code-and-ai)
* [Ghostty](https://github.com/ghostty-org/ghostty/blob/main/AI_POLICY.md)
* [Jellyfin](https://jellyfin.org/docs/general/contributing/llm-policies/)

### Organization/Company Policies
* [Oxide](https://rfd.shared.oxide.computer/rfd/0576)

### Foundation AI Policies
* [Linux Foundation](https://www.linuxfoundation.org/legal/generative-ai)
* [OpenInfra Foundation](https://openinfra.org/legal/ai-policy)


## Policy Frameworks

## Discussions
* Fedora ([discussion](https://discussion.fedoraproject.org/t/ai-policy-in-fedora-wip/144297))
* CHAOSS Augur ([discussion](https://github.com/chaoss/augur/issues/3371))
* SciPy ([discussion](https://discuss.scientific-python.org/t/a-policy-on-generative-ai-assisted-contributions/1702))
* Ansible ([discussion](https://forum.ansible.com/t/ansible-ai-policy/42642))
* pip-tools ([discussion](https://github.com/jazzband/pip-tools/discussions/2278))

### Github
* ([discussion](https://github.com/community/maintainers/discussions/470#discussioncomment-12852461))
* ([discussion](https://github.com/community/maintainers/discussions/470#discussioncomment-12390642))
* ([discussion](https://github.com/community/maintainers/discussions/442#discussioncomment-12356408))
* ([discussion](https://github.com/community/maintainers/discussions/646))


## Codes of Conduct (no specific AI mention)
* https://docs.ansible.com/ansible/latest/community/code_of_conduct.html


## Blog Posts
* https://blog.val.town/vibe-code
* https://daniel.haxx.se/blog/2025/07/14/death-by-a-thousand-slops/
* https://mitsloanedtech.mit.edu/ai/teach/ai-detectors-dont-work/
* https://www.redhat.com/en/blog/accelerating-open-source-development-ai
* https://sunnydeveloper.com/ai-consent-for-open-communities/

## News
* https://thenewstack.io/drowning-in-ai-slop-reports-curl-ends-bug-bounties/]()](https://thenewstack.io/drowning-in-ai-slop-reports-curl-ends-bug-bounties/
* 
## Tools

- PR Trust Scoring Github Action https://github.com/marketplace/actions/good-egg-trust-scoring-prs
- CHAOSS AI disclosure detection tool https://github.com/chaoss/ai-detection-action

## Other Resources
* https://github.com/adrinjalali/agents-to-block

## Responsible AI Contribution examples
* [Joshua Rogers' Curl contributions](https://mastodon.social/@bagder/115241241075258997)

## Spam examples
* [mesa contribution](https://gitlab.freedesktop.org/mesa/mesa/-/work_items/13736) ([explanation by Brodie robertson](https://www.youtube.com/watch?v=4d8jLfa5Mx8))
* https://github.com/ansible/ansible/issues/84967#issuecomment-2804372979
* https://github.com/ansible/ansible/pull/84923#issuecomment-2777540712
* https://github.com/ansible/ansible/issues/84909#issuecomment-2775920368
* [Ocaml](https://github.com/ocaml/ocaml/pull/14369): using AI tools with a niche programming language, resulting in nearly directly lifting someone elses code, including headers and attribution
* [Castle Game Engine](https://forum.castle-engine.io/t/for-you-with-ia/2048/4)  : Forum thread with "IA" where user produced code with AI that looks similar to using Castle Game Engine... but in fact is not correct.  The code is using obsolete or never-existing engine API, and (worse) goes against some of our recommended practices, in effect making the code unportable (it can only work on desktop, not mobile or web). This is problematic, as the AI code is not even a good starting point -- if you just fix it, following compiler errors, making minimal changes, you may get something that works (at least with some older engine version) but is in fact a bad starting point, not portable, not organized to scale to larger projects.
* [Submission to "modern Pascal" book](https://github.com/modern-pascal/modern-pascal-introduction/issues/28) The prose looks professional but is just factually wrong in many points. The linked issue contains also my long nice answer explaining it, so that human submitter (who wanted to do good and was just misled by AI) understands the problem.

## Credits
Thanks to the CHAOSS AI alignment working group and Sviatoslav Sydorenko for the sources that made the initial version of this list


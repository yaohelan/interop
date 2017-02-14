..

This work is licensed under a Creative Commons Attribution 3.0 Unported License.
http://creativecommons.org/licenses/by/3.0/legalcode

..
  This template should be in ReSTructured text. The filename in the git
  repository should match the launchpad URL, for example a URL of
  https://blueprints.launchpad.net/interop-workloads-specs/+spec/awesome-thing should be named
  awesome-thing.rst .  Please do not delete any of the sections in this
  template.  If you have nothing to say for a whole section, just write: None
  For help with syntax, see http://sphinx-doc.org/rest.html
  To test out your formatting, see http://www.tele3.cz/jbar/rest/rest.html

==================================
 Run vIMS on OpenStack with MANO
==================================

Include the URL of your launchpad blueprint:

https://blueprints.launchpad.net/interop-workloads/+spec/example

Network Function Virtualization(NFV) is a network architecture concept that
uses virtualization technology in Telco industry. Virtual Network Function
(VNF) is a software implementation of network functions that can be deployed
on a Network Virtualization Infrastructure(NFVI). OpenStack is a type of
NFVI. 

Running a VNF on a NFVI is a typical way to demonstrates the ability that
OpenStack supports NFV. To fulfill the goal, a NFV Management & Orchestration
(MANO) is needed to manage the lifecycle of VNF and orchestrate the services.

Here is a reference about ESTI NFV architecture
http://www.etsi.org/images/easyblog_images/NFV/NFV-blog-OPNV-initiative.png

Virtual IP Multimedia Subsystem(vIMS) network is a core component of deploying
VoLTE services in an LTE network and it a good candidate for showing the 
OpenStack deployment ability.

Problem description
===================

None

Proposed change
===============

The workload of running vIMS on OpenStack with MANO
1. Deploy 1 VM by OpenStack and install the MANO
2. Bind the MANO with OpenStack
3. Deploy the vIMS by MANO
4. Configure vIMS and set specific calling number for each OpenStack vendor
5. Show the audiences by dialing a specific number


Alternatives
------------

This is an optional section, where it does apply we'd just like a demonstration
that some thought has been put into why the proposed approach is the best one.

Implementation
==============

Assignee(s)
-----------

Who is leading the writing of the code? Or is this a blueprint where you're
throwing it out there to see who picks it up?

If more than one person is working on the implementation, please designate the
primary author and contact.

Primary assignee:
  <launchpad-id or None>

Can optionally can list additional ids if they intend on doing
substantial implementation work on this blueprint.

Milestones
----------

Target Milestone for completion:
  Juno-1

Work Items
----------

Work items or tasks -- break the feature up into the things that need to be
done to implement it. Those parts might end up being done by different people,
but we're mostly trying to understand the timeline for implementation.


Dependencies
============

- Include specific references to specs and/or blueprints in interop-workloads-specs, or in other
  projects, that this one either depends on or is related to.

- Does this feature require any new library dependencies or code otherwise not
  included in OpenStack? Or does it depend on a specific version of library?

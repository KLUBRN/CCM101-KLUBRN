# Security Audit Report

## Principle of Least Privilege (PoLP)

The Principle of Least Privilege means that each user should only receive the permissions needed to complete their assigned tasks. For example, a user who only needs to view files should not automatically have permission to delete them. This helps protect cloud accounts and prevents unnecessary access to important resources.

## Attack Surface

An attack surface is the part of a server that attackers might use to try to enter the system. It can include open network ports, active services, and applications that have security weaknesses. Keeping unused services turned off and checking which ports are accessible can help make the server harder to attack.

## Default Deny Policy

A Default Deny Policy blocks incoming connections unless a firewall rule specifically permits them. Instead of trying to identify and block every possible attacker, the administrator decides which connections are allowed to reach the server. This makes it easier to control network access and prevent unexpected connections.

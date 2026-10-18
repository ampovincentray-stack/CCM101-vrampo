# Security Audit Report

## 1. Principle of Least Privilege (PoLP)

The Principle of Least Privilege means that each user or application should receive only the permissions needed to perform its assigned tasks. In cloud environments, this reduces the damage an attacker could cause if an account or service were compromised.

## 2. Attack Surface

The attack surface of a virtual machine includes the network ports, running services, applications, and access points that an attacker could potentially target. Reducing unnecessary services and exposed ports makes it more difficult for attackers to find ways into the server.

## 3. Default Deny Policy

A Default Deny policy blocks incoming network traffic unless a specific rule permits it. This is safer than attempting to block individual attackers because unknown or unauthorized connections are blocked by default instead of being allowed until someone identifies a threat.

## 4. Security Audit Summary

The purpose of this laboratory activity is to deploy a web application, configure the Ubuntu host firewall using UFW, and permit only the required network traffic. The intended configuration blocks incoming traffic by default while allowing SSH for administration and TCP port 8080 for the web application.

## 5. Evidence

Screenshots of the running application, active firewall, and numbered firewall rules are stored in the screenshots folder.


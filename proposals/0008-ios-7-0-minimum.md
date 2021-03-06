# Base iOS Version to 7.0
* Proposal: [SDL-0008](0008-ios-7-0-minimum.md)
* Author: [Joel Fischer](https://github.com/joeljfischer)
* Status: **Accepted**
* Impacted Platforms: iOS

## Introduction
This proposal is to move the minimum iOS version allowed by iOS from 6.0 to 7.0 and to make changes taking advantage of the available iOS 7.0 APIs. Since we don't know of any major partners who currently support iOS 6.0+, we should move up our version accordingly.

## Motivation
The reason to move up to iOS 7.0 is to make available additional APIs such as `NSURLSession` and `NSURLComponents`.

## Proposed solution
In addition to moving to iOS 7.0, we should remove private classes such as `SDLURLSession` and related classes and move to `NSURLSession` which it attempts to mimic.

## Potential Downsides
Any existing app partners on iOS 6.0 would either have to drop SDL support or move to iOS 7.0+.

## Impact on existing code
This would only impact us by making available additional APIs.

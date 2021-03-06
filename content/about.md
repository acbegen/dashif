---
menu: "main"
title: "About"
weight: 2
---

In April 2012, ISO, the international standards body which had already given us
the core media foundations of MPEG-2, MP3 and MP4, finally ratified the version
of its next generation adaptive streaming standard: MPEG-DASH. In an industry
besieged by three comparable (but incompatible) segmented formats many asked
– why another? The participating companies in the MPEG-DASH standardization
(including Microsoft, Apple, Netflix, Qualcomm, Ericsson, Samsung, and many
others) saw a vision of interoperability and convergence required for
large-scale market growth that trumped the proprietary and competing solutions.
They replaced multiple corporation-controlled solutions with a single
industry-defined open standard.

In the same spirit of cooperation in which MPEG-DASH was created, the leading
streaming companies got together to form an industry forum to promote and
catalyze the adoption of MPEG-DASH and help transition it from a specification
into a real business. The DASH Industry Forum (DASH-IF) grew out of a
grassroots DASH Promoters Group and was formally incorporated in September 2012.
Today it has 67 members spread throughout the world. DASH-IF is filled with
member companies who are realists about the DASH deployment challenges. DASH by
itself is no magic panacea for the fragmentation problems of media, devices and
markets. However, the DASH-IF members do share a common vision that the
long-term benefits of convergence outweigh the costs of shorter-term efforts
involved in achieving that goal. They are willing to take on the work of
creating recommendations, filing bugs, and attending plug-fests and interop
events, with the belief that their business and the Internet streaming market
in large will benefit a great deal with convergence around DASH. The DASH-IF,
representing all sectors of the streaming media ecosystem, is proactively and
deterministically shaping the future and success of MPEG DASH.

The MPEG-DASH standard is attractive to many companies because of some key
market benefits that it brings:

- *independent stable international standard* – not owned by any single
  company, DASH is a finalized specification and not a moving target.
- *multi-video and audio tracks* – deliver the complexity of a DVD or Blu-ray
  experience, with multiple synchronized video and audio options.
- *mix of multiplexed and non-multiplexed video and audio tracks* – provide
  for dynamic bandwidth adaptation, support for multiple audio options such
  as language selection and surround sound, bandwidth efficiency (sending
  only the requested tracks) and reduced production, storage, maintenance
  and delivery costs.
- *common encryption* – one-time encryption and packaging of content allowing
  simultaneous use of multiple DRM technologies.
- *templated manifests* – Compact manifest for fast start-up, as well as
  avoiding manifest download with every segment.
- *non-segmented origin files* – files can optionally be stored contiguously
  on the server and the segments accessed via byte-range requests.
- *efficient ad insertion* – server-based and client-based targeted
  ad-insertion through the use of periods.
- *support for multiple CDNs/caches with the same manifest* – provide
  flexibility to define multiple base URL in the manifest, thus
  improving scalability and fault tolerance
- *accessibility, rating and other content descriptions* – possibility of
  signaling content descriptions such as accessibility, rating, audio
  channel configuration in the manifest.
- *industry convergence for streaming delivery* – avoid having to provide
  multiple streaming solutions, each of which requires a separate ad
  insertion flow, content protection scheme, and a different closed
  captioning format.
- *vibrant ecosystem* – already a strong community of encoders, content
  packagers, delivery platforms, and player builders has been established,
  providing a wide range of DASH solutions.
- *ease of integration* – DASH will work on any HTTP server and most
  mainstream media servers, meaning service providers and broadcast
  operators are not required to buy into new vendor-specific ecosystems
  or invest in specialized DASH-specific infrastructure.
 
One of the main challenges facing DASH after its standardization was its own
flexibility, expressed through the many features and options allowed by the
core specification. Being codec agnostic, for example, is a plus when
supporting new codec options, but poses a challenge for encoder or player
builders – which codec do you support in your DASH player? What segment
encapsulation should the encoder generate? How should DRM be signaled? What
closed captioning format do you support? The flexibility inherent in the
standard made it more difficult to achieve interoperability between various
initial implementations.

Recognizing full interoperability is the key for MPEG-DASH rapid market
adoption, the DASH-IF decided to take the raw DASH standard, marry it with a
codec, apply tight profiles and other restrictions, and create a baseline
recommendation that everyone could use to build interoperable products and
services without painful integration. Interoperability is the key to adoption
because if a format “works everywhere” then its growth will accelerate. The
name of this recommendation is “DASH-AVC/264 Implementation Guidelines” and you
can download it from https://dashif.org. It is significant because Microsoft,
Adobe, Samsung, Qualcomm, Sony, Akamai, Ericsson and 61 other members of the
DASH-IF agreed on a set of recommendations which they will support. They also
strive for compatibility with consortia standards, such as HbbTV, DECE, DTG,
HD-Forum and DLNA. DASH-IF believes that DASH-AVC/264 supports the Internet
streaming main use cases better than any existing proprietary solution.
Furthermore, DASH-IF provides conformance software, a set of test vectors, and
an open source reference client implementation for DASH-AVC/264. If you are
considering a DASH deployment, then a DASH-AVC/264 compatible solution is the
best place for you to start. For the technically inclined, here are some of the
high level key constraints that DASH-AVC/264 sets in place:

- The required video codecs are AVC/H.264 Main and High profiles. Video tracks
  using other codecs can be included.
- The required audio codec is HE-ACC v2. Audio tracks using other codecs can be
  included, including multi-channel audio.
- Segment formats are based on fragmented ISOBMFF (MP4).
- The MPEG-DASH’s “ondemand” and “live” profiles are supported.
- Segments are keyframe-aligned across representations, start with a random
  access point, and do not vary too dramatically in duration.  Therefore,
  players can switch easily between representations without having to
  download overlapping segments.
- Common Encryption is used when the content is DRM-protected.
- Closed captioning is supported using TTML-based SMPTE-TT format.
 
The advantage of an ISO standard is the openness with which it can be
evolved and improved by industry consensus. The DASH-IF is the best vector,
outside of joining MPEG directly, to propose additional features to the core
MPEG-DASH standard. Participation in DASH-IF also provides the opportunity
to collaborate with other industry leaders in developing new deployment
scenarios and corresponding implementation guidelines for MPEG-DASH. In
addition to the work done already around DASH-AVC/264, the DASH-IF has
established task forces that are actively addressing other challenging areas
of streaming:

 

*Advertising Insertion* – the recent DASH extensions provide tools for more
efficient server-side ad insertion, and make interoperable client-side ad
insertion viable. The DASH-IF Ad Insertion task force is chartered with
creating guidelines and interoperability points for both of these
architectures. The weekly task force discussions currently revolve around
mapping existing workflows into DASH and providing a capabilities gap analysis,
with a draft document expected in Q3 2013.

*DRM* – this task force focuses on interpretation of the DASH and Common
Encryption standards to identify and explain best practices and recommendations
for signaling and transmitting DRM related information in an interoperable
manner. The resulting guidelines, which are included in the DASH-AVC/264
document, explain the basic parameters and signaling mechanisms, give on
overview of a basic workflow, and show different use models for single keys
and key rotation. They also describe simple test scenarios for testing
protected content independently of proprietary DRM libraries and servers.

*Live Streaming* – Further optimization of DASH for live video services,
including Linear TV services, is one of the key features of DASH.  Due to
this workflow, additional aspects in DASH-based live service offerings need
to be taken into account to achieve interoperability, best user experience and
efficiency. The task force provides guidelines, test cases, test vectors, test
service offerings and conformance software to test interoperability for live
services. In addition, the task force looks into technical challenges and
potential enhancements for improved user experience such as lower latency,
improved audiovisual quality and supplemental features such as trick modes.

*HEVC* – High Efficiency Video Coding is the latest joint ISO MPEG and the
ITU-T video codec development with significantly improved compression rates.
HEVC was finalized in early 2013 and is expected to provide around 50%
bandwidth savings compared to AVC/H.264. Prototypes of HEVC encoding in the
combination with MPEG-DASH delivery have shown astonishing
quality-differentiating OTT. The HEVC task force addresses interoperability
and best practices aspects for HEVC delivered through DASH. The task force
collects guidelines, test cases, and test vectors to support interoperability
and demonstration efforts. Technical challenges and potential enhancements are
discussed and potentially addressed in the relevant SDOs.

*Backend Interfaces* – deploying, operating and maintaining a backend can be
costly, risky and time consuming. Having some well-defined integration points
between different providers is a clear help for facilitating such deployment.
This group is currently focusing on the interface between an encoder and the
DRM platform to facilitate and standardize the exchange of keys and DRM
metadata signals. To further increase the value of the DASH delivery ecosystem,
this group ensures that encoding protected content against multiple backend
DRM platforms is as frictionless as possible.

*Players* – there are already many companies providing DASH players for
desktop/iOS/Android use. In addition, a natural companion to DASH is the
opportunity to build HTML5 players using the Media Source Extensions and
Encrypted Media Extensions standards being defined by W3C. These browser APIs
provide a way for players, implemented purely within JavaScript, to provide
cross-platform decode and playback of adaptive, segmented content. In this
approach, the player can be downloaded as a part of the web page content and
therefore, the content provider can customize the player’s adaptation scheme
and the user experience per web page. To facilitate the use of such an approach
the DASH-IF has launched the dash.js project. dash.js provides a free, open
source DASH player which can be used as a JavaScript player or as a reference
client to implement DASH players for other platforms. Look for it on Github and
give the player a try today using Google Chrome.

We strongly believe that there is a common benefit to the entire streaming
ecosystem, from studios and operators to vendors to infrastructure providers,
in adopting DASH. We also believe that collaboration accelerates adoption.
We encourage your organization to use the DASH-IF outputs and join the DASH-IF.
Take an active part in defining, tuning, adapting and growing MPEG-DASH and
leverage its extended features to enable new applications and business use
cases. Make the streaming format of the future today’s format of choice.

[Click here](https://dashif.org/membership/) or [email](admin@dashif.org) us for more information on DASH-IF membership levels and
benefits.

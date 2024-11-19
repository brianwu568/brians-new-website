# The Drone Manifesto, Part II

This document is a work-in-progress thesis representing the evolution of my thoughts on Drone design, manufacturing, and commercial applications.

## Part II: How do we compete with foreign drone industries?

One of the major challenges for the American drone industry is getting it to compete with Chinese competitors, namely DJI. 

DJI, an acronym for “DaJiang Innovations Inc.” is a Shenzhen-based firm that is regarded as one of the largest and strongest drone manufacturers. DJI is heavily active in not only the commercial space – they are one of the largest providers of hobbyist imaging drones – but they also work very closely with the Chinese Government to supply drone-based technology solutions for the People’s Liberation Army. DJI drones, given their wide commercial availability, have been used in defense applications in many other countries, such as within the Ukraine-Russia Conflict. DJI’s origins were in its founder’s dorm room, where he built and sold drones by hand before building DJI into the empire that it is today.

It’s undeniable that DJI is the company it is today because of strong investment and support that it has received from the Chinese Government. In the United States, drone companies are often heavily regulated by the Federal Aviation Administration (FAA), which prohibits most drones from flying above 500 feet in altitude and near airports/military installations, among countless other restrictions. By contrast, DJI has been able to circumvent this in China because (1) the rules surrounding drone regulation in China are much more lax compared to the US, and (2) DJI has proven itself to be an asset for the Chinese Government such that the Chinese authorities are disincentivized to regulate the drone industry to a point where DJI begins to lose a competitive edge.

Moreover, DJI’s edge lies in that it is able to sell drones for relatively cheap prices, at least compared to any American manufacturers. Skydio’s X2 platform with enterprise-specific controllers were retailing most recently at $10,999 – way higher than DJI’s offerings, which number in the low thousands, not to mention its cheapest offering (Tello), which starts at less than $80 USD. For many price-conscious consumers, there is absolutely no reason to purchase a vastly more expensive Skydio product when a Chinese-built solution can often be available at less than 10% the cost.

If a drone manufacturer in the United States is to be as successful as DJI, then firstly it must be working directly with the government as an advocate for restrictions that do not hinder the development of such technologies – in other words, be able to rapidly prototype, iterate, and test the technology in all kinds of scenarios. Furthermore, it also must figure out a way to compete on cost, because the vast majority of buyers are willing to forgo certain features (or build some of their own, if a usable SDK is provided + the hardware is easily customizable) rather than pay an extra cost for features that they deem to be a marginal improvement. In this scenario, I’m curious whether or not a product that wins is more of a platform than a specific drone - one that involves a strong autonomy backbone and hardware shell with sensors as addons and software that can be built on top of an easy-to-use SDK.

One more challenge of Skydio’s product is that it is extremely cumbersome to use: first and foremost, the SDK itself is not publicly accessible, and must be approved via an activation code by a member of the Skydio team. This inherently limits the number of people who are able to build solutions on top of the platform, and reduces the value of the community that arises from such a setup. Furthermore, having access to the SDK is one thing; the process of programming a Skydio drone is extremely not intuitive as well. While working with a DJI Tello, I have observed two separate teams of individuals, each with a Skydio X2 platform, in which it took hours of debugging to get a drone to simply take off and hover, which is the most basic maneuver that can be performed using a drone. Finally, to top all of this off, the Skydio platform is not exactly reliable: in one scenario, where a team was trying to take off using the SDK, the software onboard the drone malfunctioned and sent constant commands for the drone to fly upwards at maximum velocity, which resulted in the drone flying in to the ceiling of the building we were testing in and shatter into pieces. Thus, in addition to a higher cost, customers face a much steeper learning curve operating Skydio drones – thus enabling us to reach the conclusion that more complex/more features is not necessarily better for drones as a product.

As discussed above, one of the core benefits we noted in customer interviews was that in addition to DJI’s cost structure (which is worth investigating more in its own right), they are able to develop class-leading autonomy and software without incurring too much development cost. This is in direct contrast to Skydio, who raised so much developmental costs as venture funding (on the magnitude of billions) and has recently announced that they had conceded the entire commercial market and would only be selling to defense. How can a future drone manufacturer avoid repeating the same mistakes that Skydio made and instead be able to compete more strongly and fairly with DJI?

My conviction is that an open platform for drones (both within software and hardware) that results in a high degree of customization is key to customer satisfaction, both within commercial and research-oriented domains. Having a SDK that is both open source and easy to use will enable the ecosystem to grow at a rapid pace; this is something that DJI has already taken advantage of by releasing Python SDKs for all of their commercial drones that enable people to program on these platforms and create more value for each other and the manufacturers by releasing open source features that enhances the operations of these drones. Furthermore, there is no reason why a quadcopter drone should be costing over five figures; it can be much cheaper to design and mass-produce a system that is robust from a hardware standpoint and contains enough sensors, compute, and power storage to perform actions such as vision or LiDAR-based SLAM. A successful player in this regard will need to work closely with the FAA and other regulatory agencies to ensure that regulations for this technology do not put us behind other countries when it comes to drone technology advancement. Non-dilutive contracts, as shown in the case of DJI, are crucial towards keeping the costs of these drones affordable and competitive with Chinese products.
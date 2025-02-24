<div class="post-header">
    <div class="post-header-background" style="background-image:url(../assets/broadmoor/gate-banner.jpg)">
        <div class="post-header-overlay">
            <h1 class="post-header-text">Liberate Broadmoor</h1>
        </div>
    </div>
</div>

# Allow bike and foot traffic through Broadmoor

_posted July 1, 2021 by [Michael Kirk](https://twitter.com/ikawe)_ &mdash;
[meet the A/B Street team](../project/team.html)

<style>
// mobile-breakpoint = 569px + --side-bar-width (300px);

#site-header {
    font-weight: 600;
    background: #f0f0f0;
    padding:12px 16px
}

#site-header-title a {
    text-decoration: none;
    font-size: 16px;
    color:#000
}

.post-header {
    position:relative;
    /* hack: mdbook doesnt support the full bleed layout we actually want, so just do something that looks decent. */
    margin-left: -15px;
    margin-right: -15px;
}

.post-header-background {
    position: relative;
    background: black;
    width: 100%;
    background-size: cover;
    background-position:center
}

.post-header-overlay {
    padding-top: 80px;
    background-color:rgba(0, 0, 0, 0.6)
}

@media (min-width: 569px) {
    .sidebar-hidden .post-header-overlay {
        padding-top:280px
    }
}

@media (min-width: 869px) {
    .sidebar-visible .post-header-overlay {
        padding-top:280px
    }
}

.post-header-text {
    color: white;
    line-height: 50px;
    font-size: 46px;
    margin: 0 16px;
    padding-bottom:16px
}

@media (min-width: calc(816px)) {
    .post-header-text {
        margin-left: auto;
        margin-right: auto;
        max-width:800px;
        /* hack: mdbook doesnt support the full bleed layout we actually want, so just do something that looks decent. */
        margin-left: 15px;
    }
}

.post-subtitle {
    margin-left: auto;
    margin-right: auto;
    max-width: 800px;
    font-style:italic
}

.post-body {
    margin-left: auto;
    margin-right: auto;
    max-width:800px
}

.media-box {
    background-color: #f0f0f0;
    color: #000;
    padding-bottom: 16px;
    margin-bottom: 16px;
    margin-top:16px
}

.media-box img {
    width:100%;
    object-fit: cover;
}

.media-box .video-container {
    width: 100%;
    position:relative
}

.media-box .embedded-video, .media-box video {
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height:100%
}

.media-box .chart-header {
    margin-top: 0;
    padding-top: 8px;
    margin-bottom: 8px;
    margin-left:16px
}

.media-box img.chart {
    padding: 8px;
    width: calc(100% - 16px);
    object-fit:contain
}

.media-box p {
    margin: 8px 16px 0 16px;
    padding:0
}

.media-box .photo-attribution {
    color: #888;
    font-size:16px
}

@media (min-width: 569px) {
    .sidebar-hidden .wrap-two {
        display: flex;
        flex-direction: row;
        justify-content:space-between
    }

    .sidebar-hidden .wrap-two .media-box:first-child {
        margin-right: 16px
    }

    .sidebar-hidden .wrap-two .media-box {
        width: 50%
    }

    .sidebar-hidden .wrap-two img {
        max-height:300px
    }
}

@media (min-width: 869px) {
    .sidebar-visible .wrap-two {
        display: flex;
        flex-direction: row;
        justify-content:space-between
    }

    .sidebar-visible .wrap-two .media-box:first-child {
        margin-right:16px
    }

    .sidebar-visible .wrap-two .media-box {
        width:50%
    }

    .sidebar-visible .wrap-two img {
        max-height:300px
    }
}


@media (max-width: 569px) {
    .sidebar-hidden .media-box {
        /* hack: mdbook doesnt support the full bleed layout we actually want, so just do something that looks decent. */
        // left: 50%;
        // margin-left: -50vw;
        // margin-right: -50vw;
        // max-width: 100vw;
        // position: relative;
        // right: 50%;
        // width:100vw
    }
}

@media (max-width: 869px) {
    .sidebar-visible .media-box {
        /* hack: mdbook doesnt support the full bleed layout we actually want, so just do something that looks decent. */
        // left: 50%;
        // margin-left: -50vw;
        // margin-right: -50vw;
        // max-width: 100vw;
        // position: relative;
        // right: 50%;
        // width:100vw
    }
}

blockquote {
    border-left: 4px solid #CCC;
    padding-left: 8px;
    margin-left: 8px
}

</style>

You could be forgiven for not knowing much about the Broadmoor neighborhood in
Seattle &mdash; that's kind of by design. We're going to explore how it could
become a valuable link for people walking and biking in Seattle, using the
travel simulation game [A/B Street](../software/abstreet.html).

<div class="media-box">
<img alt="a map of part of Seattle, highlighting the Broadmoor neighborhood, about 2.5 miles northeast of downtown." src="../assets/broadmoor/seattle-overview.png">

Broadmoor lies a few miles northeast of Downtown Seattle, sandwiched between the
[delightful Washington Park Arboretum](https://botanicgardens.uw.edu/washington-park-arboretum/)
and the Madison Park neighborhood.

</div>

Adjacent to Broadmoor, the Madison Park and Washington Park neighborhoods offer
grocery stores, a hardware store, dining, and recreational destinations.

<div class="media-box">

<img src="../assets/broadmoor/madison-park-beach.jpg" alt="a beach full of swimmers, paddle boards, and sun bathers" />

Madison Park Beach on Lake Washington is another notable neighborhood
destination.

<em class="photo-attribution">photo courtesy of the City of Seattle</em>

</div>

If you were headed to one of these destinations today, and coming from, say
Montlake or from the University District via the University bridge, it would
almost certainly require you to take a long stretch walking or biking down East
Madison Ave. This particular stretch of road is known to be
[high stress for people on bikes](https://www.seattle.gov/transportation/projects-and-programs/safety-first/vision-zero/resources/bicycle-level-of-traffic-stress),
and can be an equally harrowing walk for those on foot.

<div class="wrap-two">
<div class="media-box">
<img
  src="../assets/broadmoor/proposal-overview.png"
  alt="a proposed route, cutting through the arboretum and Broadmoor neighborhood, as opposed to a longer route possible today" />

If people were instead allowed to walk or ride through Broadmoor, they could
expect shorter trips on quieter streets.

</div>

<div class="media-box">
<img
  class="chart"
  src="../assets/broadmoor/elevation-profiles.png"
  alt="two elevation profiles, showing a gentler climb through Broadmoor" />

Looking at elevation, the green route along Madison Ave climbs an 8% grade
&mdash; quite steep! The blue route through Broadmoor offers a shorter, less
steep, route.[^elevation data]

</div>
</div>

So why don't people take this seemingly superior route through Broadmoor?
Apologies if you already have the context, but a greatly abridged history lesson
is in order for those who don't.

Up until about 200 years ago, what we refer to as Broadmoor, like much land near
the Puget Sound, was a forest inhabited by the Duwamish people. And, like much
land near the Puget Sound, it was cut clear, and the timber sold off by a mill
company. The owners of this particular parcel were the Puget Mill Company. After
logging the parcel, they split it, not quite in half. The smaller western half
was given to the city, and gardened into what is now enjoyed by the public as
the Washington Park Arboretum. The General Manager from the very same Puget Mill
Company was then allowed to develop the larger eastern half of the parcel into
that venerable American trifecta: a golf course / country club / private gated
residential community.[^madison_park_remembered]

So, Broadmoor was initially built as a gated enclave impassible to all but a
select few of the leisure class. A century later, how much has changed?

<div class="wrap-two">
<div class="media-box">
<img src="../assets/broadmoor/dead-end.jpg" alt="a sidewalk ends and a road turns where a large hedge looms" />

Try to walk through or around Broadmoor today, and you'll find yourself
repeatedly redirected or inexplicably dead-ended.

</div>

<div class="media-box">
<img src="../assets/broadmoor/front-gate.jpg" alt="a car waiting for entry at a security gate" />

There are gates on the north and south ends of Broadmoor. Both are guarded by
uniformed security.

</div>

</div>

Broadmoor is an obstacle to people walking and biking to desirable destinations
on either side of it. But what if things were different? What if we allowed
people on bikes, on foot, and in wheelchairs _through_ Broadmoor rather than
diverting them down Madison Ave?

### Cui bono

To get an intuition for the benefits that opening up Broadmoor might have, we
turn to [A/B Street](https://abstreet.org). If you have an idea for a change in
your city streets, A/B Street can visualize that change and measure its impacts.

If you've never seen A/B Street before, here's what it looks like:

<div class="media-box">
<img src="../assets/broadmoor/abstreet-overview.gif" alt="Screencast of the A/B
Street travel simulator, showing an overhead street map view, roughly centered
around the Washington Park Arboretum, with hundreds of dots sliding along the
streets. An adjustable playback speed is shown, panning and zooming in reveals
the moving dots are cartoon people and vehicles getting around the streets of
Seattle. Madison Ave looks busy.">

A/B Street uses public data sources, like
[OpenStreetMap](https://openstreetmap.org) and Seattle's
[Soundcast Travel Demand Model](https://www.psrc.org/activity-based-travel-model-soundcast)
to simulate travel in the city. You can gain insight into your proposal by
comparing metrics like travel duration and risk exposure as they are affected by
your proposal.

</div>

In A/B Street, allowing people to walk and cycle through Broadmoor, is a matter
of clicks. Then, A/B Street simulates how this change affects people's travel.
You can watch as each individual person goes about their day. If given new
circumstances, people will be able to make new, hopefully better, choices for
themselves.

To gain a little intuition for the benefits of our proposal, let's follow one
person in A/B Street on her morning walk from Madison Park to the University
District, comparing the trip before and after being allowed to walk through
Broadmoor.

<div class="media-box">

<!--
Encode the aspect ratio of the video in "padding-bottom" value. Otherwise it'll
show up letter boxed.
-->
<div class="video-container" style="padding-top: 56.25%" >
  <video controls alt="A person from the simulation exits their house in Madison park for a long walk towards the Montlake Bridge. Two routes are shown, the original route down Madison shows busy streets and several alerts as the pedestrian walks down a long stretch of Madison. The new proposed route, through Broadmoor is much calmer. The two routes converge just south of the Montlake Bridge, where the trip ends.">
    <source src="../assets/broadmoor/individual-trip-comparison.mp4" type="video/mp4">
    <source src="../assets/broadmoor/individual-trip-comparison.webm" type="video/webm">
    Sorry, your browser does not support this website's videos.
  </video>
</div>

Some of the highlights of her trip include a much calmer walk through Broadmoor
as opposed to crossing along the many busy intersections on Madison Ave.

</div>

### Beyond anecdotes

The morning commute shown above is good for story telling. It's an intuitive
anecdote for why this could be a worthwhile proposal. However, travel behavior
is highly interdependent. Every choice one person makes has potential ripple
effects for others.

We need more than a handful of individual examples. A/B Street uses Seattle's
[Soundcast travel demand model](https://www.psrc.org/activity-based-travel-model-soundcast)
to generate a realistic set of workday trips for the given area &mdash; for this
area, that's about 75,000 trips. A/B Street includes tools to analyze each of
these trips and aggregate overall travel experiences &mdash; allowing us to see
beyond anecdotes to visualize trends across the map. Let's take a look at how
overall trip times and some safety metrics are affected by this proposal.

### Trip Durations

<div class="wrap-two">
<div class="media-box">
  <h4 class="chart-header">Cars: Individual Trips</h4>
  <img class="chart" src="../assets/broadmoor/broadmoor-driving-duration-scatter.png" />

Comparing each driver's trip time before vs. after this change, some trips were a
little faster, while others a little slower.

There appears to be a small positive bias, perhaps due to less contention on
Madison, but overall it's mostly a wash for drivers, which is a boring, but
useful validation.

</div>

<div class="media-box">
  <h4 class="chart-header">Walking and Biking: Individual Trips</h4>
  <img class="chart" src="../assets/broadmoor/broadmoor-ped-bike-duration-scatter.png" />

It gets more interesting for people walking and cycling. Especially for longer
trips, people get where they're going more quickly after being allowed access
through Broadmoor, with few trips experiencing a slowdown.

</div>
</div>

Apart from the benefits conveyed to pedestrians and cyclists, these charts also
nicely show the interdependent nature of travel. For example, even though
overall travel time and the routes available to drivers didn't change much,
individual drivers did experience downstream effects of pedestrians and
bicyclists making different choices. This interdependence is fertile soil for
unintended consequences, which is why having tools to measure _overall_ impact
is essential.

<h3 class="chart-header">Time Saved / Lost</h3>

The dot charts above are helpful for seeing the shape of some trends, but it's
hard to quantify the improvements. These next charts compare the total amount of
time saved across all trips with the total amount of time lost.

<div class="wrap-two">

<div class="media-box">
  <h4 class="chart-header">Cars: Overall</h4>
  <img class="chart" src="../assets/broadmoor/broadmoor-driving-duration-histogram.png" />

Here we can confirm the small bias for faster car trips, but not much more time
is gained than was lost by others, implying a mostly neutral change across all
people driving.

</div>

<div class="media-box">
  <h4 class="chart-header">Walking and Biking: Overall</h3>
  <img class="chart" src="../assets/broadmoor/broadmoor-ped-bike-duration-histogram.png" />

A clearer trend emerges for people walking and biking &mdash; many long trips
were substantially faster given access to Broadmoor.

</div>

</div>

Trip duration is worth considering as a gut check to make sure a proposal seems
reasonable, and this proposal indeed has some favorable evidence for faster
trips, but trip duration shouldn't be the only, or even most important, effect
to consider. In particular, there are important safety metrics we can measure
with A/B Street which we'll dive into next.

## Safety

All people should be able to get where they're going safely. As our most
vulnerable road users, people walking, bicycling, and those using mobility aids
deserve extra consideration.

There is an increasing effort to not only look at previous crash sites, but also
to consider the _types_ of places where crashes are likely to occur. By
prioritizing places based on their similarity to crash sites, we can prevent or
mitigate future crash sites before someone is hurt. In this vein, last year
Seattle DOT released a
[safety study](<https://www.seattle.gov/documents/Departments/SDOT/VisionZero/SDOT_Bike%20and%20Ped%20Safety%20Analysis_Ph2_2420(0).pdf>)
analyzing which physical roadway features that are associated with an increased
risk of traffic-related death or serious injury.

For example:

> Right hook crash risk tends to be higher on arterial streets. [...] This could
> be due to the overall complexity of the intersection and/or the width of the
> intersection.[^sdot safety study]

By classifying these risky features, A/B Street can keep tabs as people in the
simulation are exposed to these risks. You can follow an individual's trip and
see what risks they are exposed to, or, for a macro view, you can aggregate and
identify map-wide hot spots for specific problems. Using A/B Street, you can
compare how a proposal affects these metrics.

<div class="wrap-two">

<div class="media-box">
<h4 class="chart-header">Identifying Hotspots</h4>
<img class="chart" 
  src="../assets/broadmoor/montlake-520-hotspot.png" 
  alt="a heatmap covering about a square mile of streets south of the Montlake
  Bridge, with hotspots on the intersections leading up to the bridge"/>

A/B Street's "problem" view helps you identify risk exposure hotspots.

These streets south of the Montlake Bridge exhibit several risk factors,
including wide streets with fast moving vehicles and many-legged intersections.

Because the Montlake Bridge is one of only a couple plausible connections
between the University District and central Seattle, it has relatively high bike
and foot traffic.

The inherent riskiness of these _kinds_ of streets, paired with the high
_number_ of people using them, results in a risk exposure hotspot worth extra
scrutiny.

</div>

<div class="media-box">
<h4 class="chart-header">Walking: Arterial Intersections</h4>
<img class="chart" 
  src="../assets/broadmoor/broadmoor-ped-arterial-crossings.png" 
  alt="2-D grid chart, bucketing trips by trip duration on the x-axis and
  number of arterial intersections crossed on the y-axis, showing a clear
  postive bias for hundreds of walking tris, especially for longer trips. Just
  a few trips were negatively affected."/>

Walking across arterial (wide, busy) intersections presents an increased risk of
death or severe injury. This chart groups walking trips by duration and by how
many fewer (or more) arterial intersections were crossed.

More than 800 walking trips had fewer arterial intersections to cross when they
were allowed to pass through Broadmoor.

The chart shows that medium-to-long trips were most affected. For example, _518_
people walking _30-60_ minutes had _1-6_ fewer arterial (major) intersections to
cross.

</div>
</div>

<div class="wrap-two">
<div class="media-box">
<h4 class="chart-header">Biking: Car Wants to Overtake</h4>
<img class="chart" 
  src="../assets/broadmoor/alerts-on-madison.gif" 
  alt="animated GIF showing an aerial map view of a simulated cyclist biking
  down the street. When a faster moving car pulls up behind them, a thought
  bubble with an alert symbol appears above the cyclist." />

A 2018 study found that most cyclists who died in single-vehicle crashes were
struck by the front of the vehicle[^fars_2018].

In shared lanes, a common risk that could lead to this type of collision is when
a faster moving car pulls up too close behind a cyclist. This is uncomfortable
for both the person on the bike and the person driving. Having the option to
ride through Broadmoor gives some cyclists the option to avoid sharing a lane
with cars on busy Madison.

</div>

<div class="media-box">
<h4 class="chart-header">Biking: Complex Intersections</h4>

<img class="chart" src="../assets/broadmoor/broadmoor-bike-complex-crossings.png" />

Simple intersections are where just two roads cross. Passing through a complex
intersection, where more than two roads cross, has an increased risk of death or
severe injury for people on bikes[^sdot safety study]. Being able to cycle
through Broadmoor was a strict improvement for this metric.

</div>
</div>

This was a quick overview of some of the tools A/B Street has for measuring
baseline safety metrics and seeing how your proposal affects them. We're
continuing to add metrics and visualizations, but we'd love to know if there are
any you'd specifically like to see.

### What's next?

Using a tool like [A/B Street](https://www.abstreet.org) is absolutely not a
definitive evaluation. It's intended to get you started tinkering.

By identifying and measuring things we care about, and simulating how they
change, we can quickly gain some visual intuition and quantified evidence to
validate (or refute) assumptions in our proposal, and hopefully it's a little
fun too.

Here we've shown there is at least some evidence that letting people walk and
bike through the Broadmoor neighborhood in Seattle could result in faster,
safer, and more pleasant trips without unduly impacting other traffic.

<!-- TODO: it'd be nice to link to something like `https://abstreet.org/web` or even http://abstreet.s3-website.us-east-2.amazonaws.com/latest/abstreet.html rather than a specific version -->

If you'd like to see for yourself what the Broadmoor proposal looks like, give
it a try,
[you can run A/B Street in your browser](http://abstreet.s3-website.us-east-2.amazonaws.com/0.2.51/abstreet.html?--dev&system/us/seattle/scenarios/arboretum/weekday.bin&--edits=broadmoor%20access)
or [download the desktop client](../user/index.html).

Or, if you have a different idea for improving how we get around, in Seattle or
elsewhere, give it a go! Please contact us on
[twitter](https://twitter.com/CarlinoDustin) or
[github](https://github.com/a-b-street/abstreet/issues/new) if you have any
questions or issues.

## Caveats

It bears repeating: A map is not the territory. The signifier is not the
signified. A simulation is not, and can never be, the actual world.

But like a good map or a good metaphor, a good simulation can be a useful tool
for learning and advocacy. Beyond the shortcomings inherent to any such semiotic
excursion, there are a couple of limitations we wanted to call out in this case
study in particular.

### Data sources

The underlying road network is inferred from
[OpenStreetMap](https://www.openstreetmap.org/#map=14/47.6337/-122.2941) (OSM),
a global community of mapping enthusiasts whose software and data is freely
available. Using OSM, A/B Street is already usable in cities all over the globe.
However, as a freely available community maintained project, OSM comes with no
data quality guarantees, and local mapping conventions can vary. Not everyone
using OSM is interested in the incredible level of detail required to run a
travel simulation. This situation is ever improving though, and we'd love to
have you give A/B Street a try, wherever you are.

A/B Street leverages Seattle's
[Soundcast travel demand model](https://www.psrc.org/activity-based-travel-model-soundcast)
to generate the list of trips for each person in A/B Street. Specifically, for
each person, Soundcast is responsible for saying where they need to be and at
what time. Soundcast is also responsible for what mode the person takes -
whether they walk, drive, cycle, etc.

### Modeshift

Intuitively if you make driving more attractive, more people will drive.
Similarly if you make a mode like cycling, walking, or transit more attractive,
more people will choose that mode.

A/B Street doesn't currently account for this shifting of modes. It naively
assumes that people will go about their day, always choosing to drive or walk or
cycle regardless of what changes you make to the city. Mode shift is a real and
important behavior that we are excited to implement and measure in A/B Street in
the future.

There's tons of other improvements in the works. Follow
[@CarlinoDustin](https://twitter.com/CarlinoDustin) for updates, and let us know
what you'd like to see.

## Footnotes

<!-- prettier-ignore-start -->
[^elevation data]:
Elevation data from [King County LIDAR](http://pugetsoundlidar.ess.washington.edu/lidardata/restricted/projects/2016king_county.html). Thanks to [Eldan Goldenberg](https://github.com/eldang/elevation_lookups) for processing this data.

[^madison_park_remembered]: Jane Powell Thomas, Madison Park Remembered (J.P. Thomas, 2004)

[^sdot safety study]: Seattle Department of Transportation's safety study:
[City of Seattle Bicycle and Pedestrian Safety Analysis Phase&nbsp;2](https://www.seattle.gov/documents/Departments/SDOT/VisionZero/SDOT_Bike%20and%20Ped%20Safety%20Analysis_Ph2_2420(0).pdf)

[^fars_2018]: NHTSA | National Highway Traffic Safety Administration - [2018 Traffic Safety Facts](https://crashstats.nhtsa.dot.gov/Api/Public/ViewPublication/812884)

<!-- prettier-ignore-end-->

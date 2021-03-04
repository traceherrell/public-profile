<script>
    import ls1 from "images/launchstudio.png";
    import ls2 from "images/launchstudio-newproject.png";
    import ls3 from "images/launchstudio-search.png";
    import ls4 from "images/tcm2.png";
    import ls5 from "images/tcm3.png";
    import jls1 from "images/j_search.png";

    import {
        Button,
        Card,
        CardBody,
        Carousel,
        CarouselItem,
        CarouselIndicators,
        CarouselControl,
        CarouselCaption,
        Modal,
    } from "sveltestrap/src";
    let open = false;
    const toggle = () => (open = !open);

    const items = [
        {
            url: ls2,

            title: "Slide 1",
            subTitle: "Slide 1",
        },
        {
            url: ls3,
            title: "Slide 2",
            subTitle: "Slide 2",
        },
        {
            url: ls4,
            title: "Slide 3",
            subTitle: "Slide 3",
        },
        {
            url: ls5,
            title: "Slide 4",
            subTitle: "Slide 4",
        },
    ];

    let activeIndex = 0;
</script>

<svelte:head>
    <title>Trace Herrell - Portfolio</title>
</svelte:head>

<div class="container">
    <div class="row">
        <div class="col-md-6">
            <div class="card" style="width: 20rem;">
                <img
                    class="card-img-top img-fluid"
                    src={ls1}
                    alt="Launch Studio"
                />
                <div class="card-body">
                    <h4 class="card-title">Bluetooth Launch Studio</h4>
                    <p class="card-text">
                        A tool to complete the Bluetooth qualification process.
                        This tool is only for bluetooth members so I can't link
                        directly to the application. Click below to view some
                        screens.
                    </p>
                    <Button color="primary" on:click={toggle}
                        >View Screen Shots</Button
                    >
                </div>
            </div>
        </div>
        <div class="col-md-6">
            <div class="card" style="width: 20rem;">
                <img
                    class="card-img-top img-fluid"
                    src={jls1}
                    alt="John L Scott"
                />
                <div class="card-body">
                    <h4 class="card-title">John L Scott</h4>
                    <p class="card-text">
                        Search and find realestate listings similar to Redfin
                        and Zillow. Since this is a public site you can click
                        the button below to try it out yourself.
                    </p>
                    <a
                        href="https://www.johnlscott.com/search"
                        class="btn btn-primary">JohnLScott.com</a
                    >
                </div>
            </div>
        </div>
    </div>
    <div>
        <!-- Modal Component -->
        <Modal isOpen={open} {toggle} size="lg" title="Bluetooth Launch Studio">
            <Carousel {items} bind:activeIndex ride={true} interval={2000}>
               
                <div class="carousel-inner">
                    {#each items as item, index}
                        <CarouselItem bind:activeIndex itemIndex={index}>
                            <img
                                src={item.url}
                                class="d-block w-100"
                                alt={item.title}
                            />
                            <CarouselCaption
                                captionHeader={item.title}
                                captionText={item.subTitle}
                            />
                        </CarouselItem>
                    {/each}
                </div>

                <CarouselControl direction="prev" bind:activeIndex {items} />
                <CarouselControl direction="next" bind:activeIndex {items} />
            </Carousel>
        </Modal>
    </div>
</div>

<style>
    .card {
        margin-top: 50px;

        float: left;
    }
</style>

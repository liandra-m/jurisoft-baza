<script setup>
    import { FontAwesomeIcon } from '@fortawesome/vue-fontawesome';
    import {library} from '@fortawesome/fontawesome-svg-core';
    import {faCircleCheck, faCircleQuestion} from '@fortawesome/free-solid-svg-icons';

    library.add(faCircleCheck);
    library.add(faCircleQuestion);
</script>

<template>
  <div class="page content">
    <section class="landing">
      <h1>
        Think less about <br />
        tracking numbers, more <br />
        about your business.
      </h1>

      <span>
        Our app will help you to save time on tracking the activity, time,
        <br />
        earnings and more. Take everything under control with Baza.
      </span>

      <div class="actions">
        <button class="btn btn-primary box-shadow btn-min">Get started</button>
        <button class="btn btn-secondary btn-min">Learn more</button>
      </div>

      <div class="img-wrapper box-shadow">
        <img src="/images/3.png" />
      </div>
    </section>

    <section class="benefits grid">
      <div>
        <img src="/images/4.png" />
        <h2>Time tracking</h2>
        <span>
          Our app will help you to save time on tracking the activity, time,
          earnings and more. Any time you can be sure everything is under your
          control.
        </span>
      </div>

      <div>
        <img src="/images/5.png" />
        <h2>Activity monitoring</h2>
        <span>
          Our app will help you to save time on tracking the activity, time,
          earnings and more. Any time you can be sure everything is under your
          control
        </span>
      </div>

      <div>
        <img src="/images/10.png" />
        <h2>Generating reports</h2>
        <span>
          Our app will help you to save time on tracking the activity, time,
          earnings and more. Any time you can be sure everything is under your
          control
        </span>
      </div>
    </section>

    <div class="platform-detail">
      <div class="column max-w align-base">
        <h2>Accurate and easy platform for productivity tracking</h2>
        <span>
          Our app will help you to save time on tracking the activity, time,
          earnings and more. Take everything under control with Baza.
        </span>
        <button style="margin-top: 25px" class="btn btn-primary box-shadow">Get started</button>
      </div>

        <div class="img-wrapper">
            <img src="/images/6.png" />
        </div>
    </div>

    <section class="bg-white">
      <section class="stats grid">
        <div>
          <h2>90K</h2>
          <span> Active users </span>
        </div>

        <div>
          <h2>62M+</h2>
          <span> Tasks completed </span>
        </div>

        <div>
          <h2>68K</h2>
          <span> Reports generated </span>
        </div>
      </section>

      <section class="steps">
        <div class="title">
            <h2>Improve team productivity</h2>
            <span>
                Our app will help you to save time on tracking the activity, time,
                earnings and more. Take everything under control with Baza.
            </span>
        </div>

        <div class="flex platform-detail">
            <div class="img-wrapper">
                <img src="/images/7.png" />
            </div>
            <ul>
                <li>
                    <font-awesome-icon :icon="['fa','circle-check']" />
                    <div>
                        <h2>Install the app</h2>
                        <span>
                            Easy to install the app, no specific skills needed.
                            Take everything under control with Baza.
                        </span>
                    </div>
                </li>
                <li>
                    <font-awesome-icon :icon="['fa','circle-check']" />
                    <div>
                        <h2>Set the goals</h2>
                        <span>
                            Easy to install the app, no specific skills needed.
                            Take everything under control with Baza.
                        </span>
                    </div>
                </li>
                <li>
                    <font-awesome-icon :icon="['fa','circle-check']" />
                    <div>
                        <h2>Create tasks</h2>
                        <span>
                            Easy to install the app, no specific skills needed.
                            Take everything under control with Baza.
                        </span>
                    </div>
                </li>
            </ul>
        </div>
      </section>
      
    <section class="reviews">
        <div class="platform-detail">
            <div class="review">
                <div class="profile">
                    <img src="/images/9.png" />
                </div>

                <h2>"Best Choice!"</h2>
                <span>
                    Everything is done perfectly and we can finish our projects on time
                    from now on.
                </span>

                <h3>Mat Goldman</h3>
                <span>Developer</span>
            </div>

            <div class="review">
                <div class="profile">
                    <img src="/images/8.png" />
                </div>

                <h2>"Happy CEO, happy team"</h2>
                <span>
                    I am happy that i chose Baza to work with my remote team.
                </span>

                <h3>Max Smit</h3>
                <span>CEO of Fast Tech</span>
            </div>

        </div>
    </section>

    <section class="pricing">
        <div class="title">
            <h2>Our pricing</h2>
            <p>
                Our app will help you to save time on tracking the activity, time,
                earnings and more. Take everything under control with Baza.
            </p>
        </div>

        <div class="grid">
            <div class="price-box">
                <p class="tag">LITE</p>
                
                <h2 style="font-size: 48px;">10$</h2>
                <span style="color: var(--primary-color)">monthly payment</span>

                <ul>
                    <li>
                        <font-awesome-icon class="grey-variant" :icon="['fa','circle-check']" />
                        <div>
                            <h3>Time tracking</h3>
                        </div>
                    </li>
                    <li>
                        <font-awesome-icon class="grey-variant" :icon="['fa','circle-check']" />
                        <div>
                            <h3>Activity monitoring</h3>
                        </div>
                    </li>
                    <li class="disabled">
                        <font-awesome-icon class="grey-variant" :icon="['fa','circle-check']" />
                        <div>
                            <h3>Generating reports</h3>
                        </div>
                    </li>
                    <li class="disabled">
                        <font-awesome-icon class="grey-variant" :icon="['fa','circle-check']" />
                        <div>
                            <h3>Company analytics</h3>
                        </div>
                    </li>
                </ul>

                <button class="btn btn-primary box-shadow" style="margin-top: 40px; padding: 15px 75px; align-self: center;">Get started</button>
            </div>

                <div class="price-box">
                <p class="tag">PRO</p>
                
                <h2 style="font-size: 48px;">30$</h2>
                <span style="color: var(--primary-color)">monthly payment</span>

                <ul>
                    <li>
                        <font-awesome-icon class="grey-variant" :icon="['fa','circle-check']" />
                        <div>
                            <h3>Time tracking</h3>
                        </div>
                    </li>
                    <li>
                        <font-awesome-icon class="grey-variant" :icon="['fa','circle-check']" />
                        <div>
                            <h3>Activity monitoring</h3>
                        </div>
                    </li>
                    <li>
                        <font-awesome-icon class="grey-variant" :icon="['fa','circle-check']" />
                        <div>
                            <h3>Generating reports</h3>
                        </div>
                    </li>
                    <li class="disabled">
                        <font-awesome-icon class="grey-variant" :icon="['fa','circle-check']" />
                        <div>
                            <h3>Company analytics</h3>
                        </div>
                    </li>
                </ul>

                <button class="btn btn-primary box-shadow" style="margin-top: 40px; padding: 15px 75px; align-self: center;">Get started</button>
            </div>

            <div class="price-box">
                <p class="tag">BUSINESS</p>
                
                <h2 style="font-size: 48px;">80$</h2>
                <span style="color: var(--primary-color)">monthly payment</span>

                <ul>
                    <li>
                        <font-awesome-icon class="grey-variant" :icon="['fa','circle-check']" />
                        <div>
                            <h3>Time tracking</h3>
                        </div>
                    </li>
                    <li>
                        <font-awesome-icon class="grey-variant" :icon="['fa','circle-check']" />
                        <div>
                            <h3>Activity monitoring</h3>
                        </div>
                    </li>
                    <li>
                        <font-awesome-icon class="grey-variant" :icon="['fa','circle-check']" />
                        <div>
                            <h3>Generating reports</h3>
                        </div>
                    </li>
                    <li>
                        <font-awesome-icon class="grey-variant" :icon="['fa','circle-check']" />
                        <div>
                            <h3>Company analytics</h3>
                        </div>
                    </li>
                </ul>

                <button class="btn btn-primary box-shadow" style="margin-top: 40px; padding: 15px 75px; align-self: center;">Get started</button>
            </div>

        </div>

        <div class="doubts grid">
            <div class="column">
                <div class="flex">
                    <font-awesome-icon class="green-variant" :icon="['fa','circle-question']" />
                    <div>
                        <h2>
                            How does app work?
                        </h2>
                        <p>
                            Easy to install the app, no specific skills needed.
                            Take everything under control with Baza.
                        </p>
                    </div>
                </div>

                <div class="flex">
                    <font-awesome-icon class="green-variant" :icon="['fa','circle-question']" />
                    <div>
                        <h2>
                            Which operating systems is app compatible with?
                        </h2>
                        <p>
                            Easy to install the app, no specific skills needed.
                            Take everything under control with Baza.
                        </p>
                    </div>
                </div>

                <div class="flex">
                    <font-awesome-icon class="green-variant" :icon="['fa','circle-question']" />
                    <div>
                        <h2>
                            How can i get report?
                        </h2>
                        <p>
                            Easy to install the app, no specific skills needed.
                            Take everything under control with Baza.
                        </p>
                    </div>
                </div>
            </div>

            <div class="column">
                <div class="flex">
                    <font-awesome-icon class="green-variant" :icon="['fa','circle-question']" />
                    <div>
                        <h2>
                            How does app work?
                        </h2>
                        <p>
                            Easy to install the app, no specific skills needed.
                            Take everything under control with Baza.
                        </p>
                    </div>
                </div>

                <div class="flex">
                    <font-awesome-icon class="green-variant" :icon="['fa','circle-question']" />
                    <div>
                        <h2>
                            Which operating systems is app compatible with?
                        </h2>
                        <p>
                            Easy to install the app, no specific skills needed.
                            Take everything under control with Baza.
                        </p>
                    </div>
                </div>

                <div class="flex">
                    <font-awesome-icon class="green-variant" :icon="['fa','circle-question']" />
                    <div>
                        <h2>
                            How can i get report?
                        </h2>
                        <p>
                            Easy to install the app, no specific skills needed.
                            Take everything under control with Baza.
                        </p>
                    </div>
                </div>
            </div>

        </div>

        <p style="margin-top: 30px">
            Didn't find your answer? <a class="green-variant" href="#contact">Contact us now</a>
        </p>
    </section>

    <section class="footer">
        <div class="column">
            <div class="footer-content">
                <div class="img-wrapper">
                    <img src="/images/2.png" />
                </div>
                <div class="text">
                    <h2>Ready to improve productivity?</h2>
                    <p>
                        Our app will help you to save time on tracking the activity, time,
                        earnings and more. Take everyhint under control with Baza.
                    </p>
                </div>
                <div>
                    <button class="btn btn-primary box-shadow">Get started</button>
                </div>
            </div>
            
        </div>
    </section>

    <section class="footer-info">
        <span>Copyright @2022 Baza. All rights reserved.</span>
        <ul>
            <li>
                <a href="#news">
                    Whats New  
                </a>
            </li>

            <li>
                <a href="#sell">
                    Sell Online
                </a>
            </li>

            <li>
                <a href="#blog">
                    Blog
                </a>
            </li>

            <li>
                <a href="#contact">
                    Contact Us
                </a>
            </li>
        </ul>
    </section>

    </section>

    <div class="wrapper">
        <img class="right-img" src="/images/1.png" />
    </div>
    
    <img class="left-img" src="/images/11.png" />
  </div>
</template>

<style scoped>
    @import "./page.css";
    @import "./responsive.css";
</style>

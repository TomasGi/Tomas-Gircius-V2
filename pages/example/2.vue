<template>
    <div>
        <div class="container">
            <div class="carousel-holder">
                <client-only placeholder="Loading...">
                    <carousel :data="slides"></carousel>
                </client-only>
            </div>
            <div class="list">
                <div class="item">
                    <h3>Work done</h3>
                    <ul>
                        <li>design development</li>
                        <li>translations</li>
                        <li>shared hosting server configuration</li>
                        <li>frontend development</li>
                    </ul>
                </div>
                <div class="item">
                    <h4>Tech used</h4>
                    <ul>
                        <li>nuxt.js static</li>
                        <li>vue</li>
                        <li>i18n.js</li>
                    </ul>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    data() {
        // let count = 3;
        // let src = '/images/vait/';
        // let slides = [];

        // for (let i = 1; i < count + 1; i++) {
        //     slides[i] = {
        //         id: i,
        //         content(createElement, content) {
        //             return createElement('div', {
        //                 attrs: {
        //                     class: 'slide'
        //                 }
        //             }, [
        //                 createElement('img', {
        //                     attrs: {
        //                         src: `${src + i}.jpg`
        //                     }
        //                 })
        //             ])
        //         }
        //     }
        // }

        return {
            slides: [
                {
                    id: 1,
                    content(createElement, content) {
                    return createElement('div', {
                        attrs: {
                            class: 'slide'
                        }
                    }, [
                            createElement('img', {
                                attrs: {
                                    src: 'images/vait/1.jpg'
                                }
                            })
                        ])
                    }
                },
                {
                    id: 2,
                    content(createElement, content) {
                    return createElement('div', {
                        attrs: {
                            class: 'slide'
                        }
                    }, [
                            createElement('img', {
                                attrs: {
                                    src: 'images/vait/2.jpg'
                                }
                            })
                        ])
                    }
                },
                {
                    id: 3,
                    content(createElement, content) {
                    return createElement('div', {
                        attrs: {
                            class: 'slide'
                        }
                    }, [
                            createElement('img', {
                                attrs: {
                                    src: 'images/vait/3.jpg'
                                }
                            })
                        ])
                    }
                }
            ]
        }
    }
};
</script>
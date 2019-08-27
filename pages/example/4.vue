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
                    <h4>Some logos</h4>
                    <h4>Tech used</h4>
                    <ul>
                        <li>Adobe Illustrator</li>
                        <li>Adobe Photoshop</li>
                    </ul>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    data() {
        // let count = 6;
        // let src = '/images/log/';
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
                                    src: '/images/log/1.jpg'
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
                                    src: '/images/log/2.jpg'
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
                                    src: '/images/log/3.jpg'
                                }
                            })
                        ])
                    }
                },
                {
                    id: 4,
                    content(createElement, content) {
                    return createElement('div', {
                        attrs: {
                            class: 'slide'
                        }
                    }, [
                            createElement('img', {
                                attrs: {
                                    src: '/images/log/4.jpg'
                                }
                            })
                        ])
                    }
                },
                {
                    id: 5,
                    content(createElement, content) {
                    return createElement('div', {
                        attrs: {
                            class: 'slide'
                        }
                    }, [
                            createElement('img', {
                                attrs: {
                                    src: '/images/log/5.jpg'
                                }
                            })
                        ])
                    }
                },
                {
                    id: 6,
                    content(createElement, content) {
                    return createElement('div', {
                        attrs: {
                            class: 'slide'
                        }
                    }, [
                            createElement('img', {
                                attrs: {
                                    src: '/images/log/6.jpg'
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
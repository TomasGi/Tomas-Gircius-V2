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
                        <li>backend development</li>
                        <li>frontend development</li>
                    </ul>
                </div>
                <div class="item">
                    <h4>Tech used</h4>
                    <ul>
                        <li>symfony 3.4+</li>
                    </ul>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    data() {
        // let count = 4;
        // let src = '/images/sam/';
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
                                    src: '/images/sam/1.jpg'
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
                                    src: '/images/sam/2.jpg'
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
                                    src: '/images/sam/3.jpg'
                                }
                            })
                        ])
                    }
                }
                ,
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
                                    src: '/images/sam/4.jpg'
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
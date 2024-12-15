<!DOCTYPE html>
<html lang="en">
    <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title>我的简历</title>
        <style>
            :root {
                --color-white: #FFFFFF;
                --color-black: #000000;
                --color-darkgray: #333333;
                --color-gray: #5D5D5D;
                --color-lightgray: #999999;
                --color-text: var(--color-darkgray);
                --color-graytext: var(--color-gray);
                --color-lighttext: var(--color-lightgray);
                --color-awesome: #DC3522;
                 --color-yellow: #FFC107; /* 黄色 */
                --font-size-base: 16px;
                --spacing-unit: 1rem;
            }

            * {
                margin: 0;
                padding: 0;
                box-sizing: border-box;
            }

            body {
                font-family: 'Source Sans Pro', sans-serif;
                font-size: var(--font-size-base);
                line-height: 1.5;
                color: var(--color-yellow);
                background: var(--color-white);
                padding: 2rem;
                max-width: 1200px;
                margin: 0 auto;
            }

            /* .cv-header {
                text-align: center;
                margin-bottom: 2rem;
            } */

            .cv-name {
                display: flex;
                justify-content: center;
                align-items: baseline;
                gap: 0.5rem;
                margin-bottom: 1rem;
            }

            .firstname {
                font-size: 2rem;
                font-weight: 300;
                color: var(--color-graytext);
            }

            .lastname {
                font-size: 2rem;
                font-weight: 300;
                color: var(--color-text);
            }

            .position {
                font-size: 0.9rem;
                text-transform: uppercase;
                color: var(--color-yellow);
                margin-bottom: 0.5rem;
            }

            .contact-info {
                font-size: 0.8rem;
                color: var(--color-lighttext);
            }

            .section {
                margin-bottom: 2rem;
            }

            .section-title {
                font-size: 1.25rem;
                font-weight: 700;
                color: var(--color-yellow);
                text-transform: uppercase;
                margin-bottom: 1rem;
                position: relative;
            }

            .section-title::after {
                content: '';
                position: absolute;
                left: 0;
                bottom: -0.25rem;
                width: 100%;
                height: 0.15rem;
                background-color: var(--color-yellow);
                opacity: 0.3;
            }
            .section-title2 {
                color: red; /* 设置文本颜色为红色 */
                font-size: 7rem;
            }

            .entry {
                margin-bottom: 1.5rem;
            }

            .entry-title {
                font-weight: 700;
                margin-bottom: 0.25rem;
            }
            .entry-title-small {
                font-weight: 500;
                margin-bottom: 0.25rem;
            }

            .entry-info {
                display: flex;
                justify-content: space-between;
                font-size: 0.9rem;
                color: var(--color-graytext);
                margin-bottom: 0.5rem;
            }

            .entry-info2 {
                display: flex;
                justify-content: space-between;
                font-size: 3rem;
                color: var(--color-graytext);
                margin-bottom: 0.5rem;
            }

            .entry-description {
                font-size: 0.9rem;
                color: var(--color-text);
            }

            @media (max-width: 768px) {
                body {
                    padding: 1rem;
                }

                .entry-info {
                    flex-direction: column;
                    gap: 0.25rem;
                }
            }
            .blue-link {
                color: yellow;
                text-decoration: none; /* 移除下划线 */
            }
            .blue-link:hover {
                text-decoration: underline; /* 悬停时显示下划线 */
            }
            .cv-header {
                text-align: center;
                margin-bottom: 2rem;
                position: relative;
                padding: 1rem;
            }

            .photo-container {
                width: 120px;
                height: 120px;
                position: absolute;
                overflow: hidden;
            }

            .photo-container.left {
                left: 0;
            }

            .photo-container.right {
                right: 0;
            }

            .photo-container.circle {
                border-radius: 50%;
            }

            .photo-container.rectangle {
                border-radius: 3px;
            }

            .photo-container.edge {
                border: 3px solid var(--color-yellow);
            }

            .photo-container img {
                width: 100%;
                height: 100%;
                object-fit: cover;
            }

            /* Adjust header layout when photo is present */
            .has-photo {
                padding-left: 140px; /* When photo is on the left */
            }

            .has-photo.photo-right {
                padding-left: 0;
                padding-right: 140px;
            }

            @media (max-width: 768px) {
                .cv-header {
                    padding: 0;
                }

                .photo-container {
                    position: relative;
                    margin: 0 auto 1rem auto;
                }

                .has-photo, .has-photo.photo-right {
                    padding: 0;
                }
            }
        </style>
    </head>
    <body>
        <header class="cv-header">
            <!-- Photo container with configurable options -->
            <div class="photo-container left circle edge">
                <!-- Replace src with actual photo path -->
                <img src="微信图片_20241215183601.jpg" alt="Profile Photo">
            </div>
            <div class="cv-name">
                <span class="firstname">檀</span>
                <span class="lastname">健次</span>
            </div>
            <div class="position">中国内地男演员、歌手</div>
            <div class="contact-info">
                📍 北京体育大学• 🧣 MIC檀健次JC-T • 📧 JCTStudio@163.com（工作）JCT Fans@163.com（粉丝）
            </div>
        </header>

        <main>
            <section class="section">
                <h2 class="section-title">基本信息</h2>
                <div class="entry">
                    <div class="entry-info">
                        <span>  檀健次，1990年10月5日出生于广西壮族自治区北海市，中国内地影视男演员、流行乐歌手，毕业于北京体育大学体育舞蹈专业。
                            2007年，主演个人首部电影《秘岸》并被唱片公司选中成为练习生，经历四年封闭训练，
                            2010年以MIC男团成员身份正式出道。
                            2014年，发行个人首支音乐单曲《Fly Away》。
                            2016年，出演古装剧《大军师司马懿之军师联盟》和其续集《虎啸龙吟》，饰演司马昭。2018年，参加演技竞演类节目《我就是演员》，以演员身份获得认可。
                            2018年至2021年，出演《三国机密之潜龙在渊》《鬓边不是海棠红》《爱的厘米》等多部影视作品。
                            2020年，参加男性音乐竞演综艺节目《追光吧！哥哥》，最终成为“追光之星”并获得“年度追光之星”的称号。
                            2022年3月，首次担任男一号主演的刑侦探案剧《猎罪图鉴》播出，饰演画像师沈翊，收获广泛关注和口碑；5月，加盟综艺节目《你好，星期六》担任“好6团”成员；
                            9月，主演的网络安全题材悬疑剧《你安全吗》播出。2023年4月，发行个人首张音乐专辑《DREAMS》；7月，在爱情奇幻古装剧《长相思》中分饰九头蛇妖相柳和防风邶两角，收获大量人气；
                            11月，主演的新国风声恋剧《很想很想你》播出。2024年3月，主演的爱情电影《被我弄丢的你》上映；6月，发行第二张个人专辑《焕》，并于同月官宣首次个人巡回演唱会《多见一次》。</span>

                    </div>

                </div>
            </section>


            <section class="section">
                <h2 class="section-title">获奖经历</h2>
                <div class="entry">
                    <div class="entry-info">
                        <span>2024微博视界大会年度质感演绎</span>
                    </div>
                    <div class="entry-info">
                        <span>2024微博视界大会年度推荐·观众喜爱荣耀</span>
                    </div>
                     <div class="entry-info">
                        <span>2024微博视界大会大学生年度推荐·影视角色</span>
                    </div>
                    <div class="entry-info">
                        <span>2023微博之夜微博年度瞩目演员</span>
                    </div>
                    <div class="entry-info">
                        <span>2023腾讯视频星光大赏年度全能艺人</span>
                    </div>
                    <div class="entry-info">
                        <span>2023微博视界大会年度号召力演员</span>
                    </div>
                     <div class="entry-info">
                        <span>……</span>
                    </div>
                </div>
            </section>
             <section class="section">
                <h2 class="section-title2">热播新剧</h2>
                <div class="entry-info2">
                    <span>《猎罪图鉴2》正在爱奇艺和腾讯视频热播中！！！点击下方链接即刻观看</span>
                </div>
                 <div class="entry-info2">
                     <a href="https://v.qq.com/x/cover/mzc00200mnco4mw/p4100lv2bw4.html" target="_blank">https://v.qq.com/x/cover/mzc00200mnco4mw/p4100lv2bw4.html</a>
                 </div>
                 <div class="entry-info2">
                     <a href="https://www.iqiyi.com/v_1pkjkyp9rvk.html?vfrm=pcw_album_auto&rfr=https://cn.bing.com/" target="_blank">https://www.iqiyi.com/v_1pkjkyp9rvk.html?vfrm=pcw_album_auto&rfr=https://cn.bing.com/</a>
                 </div>
        </main>
    </body>

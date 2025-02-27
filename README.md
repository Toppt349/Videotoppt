<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>My Video Gallery</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #181818;
            color: white;
            margin: 0;
            padding: 20px;
        }

        h1 {
            text-align: center;
            margin-bottom: 20px;
        }

        .search-container {
            text-align: center;
            margin-bottom: 20px;
        }

        .search-box {
            padding: 10px;
            width: 300px;
            border-radius: 5px;
            border: none;
            font-size: 16px;
        }

        .video-container {
            display: flex; 
            overflow-x: auto; 
            gap: 20px;
            padding-bottom: 20px; 
        }

        .video-box {
            background: #202020;
            padding: 10px;
            border-radius: 10px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.3);
            transition: transform 0.3s ease;
            min-width: 320px; 
        }

        .video-box:hover {
            transform: scale(1.05);
        }

        iframe {
            width: 100%;
            height: 180px;
            border-radius: 10px;
            border: none;
        }

        .video-title {
            margin-top: 10px;
            font-size: 16px;
            font-weight: bold;
            text-align: center;
        }

        /* Responsive styles */
        @media (max-width: 768px) {
            iframe {
                height: 200px;
            }

            .video-title {
                font-size: 14px;
            }

            h1 {
                font-size: 24px;
            }
        }

        @media (max-width: 480px) {
            iframe {
                height: 160px;
            }

            .video-title {
                font-size: 12px;
            }

            h1 {
                font-size: 20px;
            }
        }
    </style>
    <h1>🎥 Anime H Gallery</h1>

    <!-- Search Bar -->
    <div class="search-container">
        <input type="text" id="searchInput" class="search-box" placeholder="Search Videos..." oninput="filterVideos()">
    </div>

    <!-- Video Containers -->
    <div class="video-container" id="videoContainer1">
        <div class="video-box" data-title="Machi-1">
            <iframe src="https://drive.google.com/file/d/1v_PcupEWHj-DZ1rC7CvMG0xh2Gge_TPU/preview" allow="autoplay"></iframe>
            <div class="video-title">Video 1</div>
        </div>

        <div class="video-box" data-title="HonkaiImpact-2">
            <iframe src="https://drive.google.com/file/d/1zpBDTn28jPtmZH59HgNXS-jToSoB2oOu/preview" allow="autoplay"></iframe>
            <div class="video-title">Video 2</div>
        </div>

        <div class="video-box" data-title="Mika-bluearchive-3">
            <iframe src="https://drive.google.com/file/d/1uBgqAHaDKggp6AyOXQ9oh0sZz6t18btH/preview" allow="autoplay"></iframe>
            <div class="video-title">Video 3</div>
        </div>

        <div class="video-box" data-title="Raiden-Genshin-4">
            <iframe src="https://drive.google.com/file/d/1AiLE5aP4VqSOMEUPcGYzrbbedEnnUxBa/preview" allow="autoplay"></iframe>
            <div class="video-title">Video 4</div>
        </div>
        
        <div class="video-box" data-title="Video 5-5">
            <iframe src="https://drive.google.com/file/d/1WuKp5qZcT_tnqD7gtVFiaXfavnnB1twf/preview" allow="autoplay"></iframe>
            <div class="video-title">Video 5</div>
        </div>

        <div class="video-box" data-title="Tosaka-Chicken-6">
            <iframe src="https://drive.google.com/file/d/10OUoaOaRNzervFJhp-rSroPuuW-Wh0pY/preview" allow="autoplay"></iframe>
            <div class="video-title">Video 6</div>
        </div>

        <div class="video-box" data-title="Tosaka-Chicken-7">
            <iframe src="https://drive.google.com/file/d/1lCb6oJbfDZZsfYFUkrq41b9Kp5609UO_/preview" allow="autoplay"></iframe>
            <div class="video-title">Video 7</div>
        </div>

        <div class="video-box" data-title="Vtuber-8">
            <iframe src="https://drive.google.com/file/d/1ZSPsXJd4mdecjMyhQHTNrZE8Q91BYJmd/preview" allow="autoplay"></iframe>
            <div class="video-title">Video 8</div>
        </div>

        <div class="video-box" data-title="Janedoe-zzz-9">
            <iframe src="https://drive.google.com/file/d/18ZDPA76vRGQecI_Xt_C6-2zh1OIhr3Pe/preview" allow="autoplay"></iframe>
            <div class="video-title">Video 9</div>
        </div>

        <div class="video-box" data-title="zzz-10">
            <iframe src="https://drive.google.com/file/d/1EK7C7XDORlEbTHPY_U1nBlhKmf-tGHo9/preview" allow="autoplay"></iframe>
            <div class="video-title">Video 10</div>
        </div>
    </div>

    <div class="video-container" id="videoContainer2">
        <div class="video-box" data-title="RaidenMei-Honkaistaril-Machi-11">
            <iframe src="https://drive.google.com/file/d/1e_9O1LALphMqZkdnYHLwfNoRhHeQ3JhE/preview" allow="autoplay"></iframe>
            <div class="video-title">Video 11</div>
        </div>
        <div class="video-box" data-title="Reelruru-12">
            <iframe src="https://drive.google.com/file/d/15V7eOeGesVKUPCFwpFuE_0O_LWCxhkNG/preview" allow="autoplay"></iframe>
            <div class="video-title">Video 12</div>
        </div>
        <div class="video-box" data-title="Ako-bluearchive-13">
            <iframe src="https://drive.google.com/file/d/1WPq7-dQW5XJTmBEznsTdJ76L4TLWhoQ0/preview" allow="autoplay"></iframe>
            <div class="video-title">Video 13</div>
        </div>
        <div class="video-box" data-title="Ako-bluearchive-14">
            <iframe src="https://drive.google.com/file/d/1AHE2gnyFb3Vk-tYjUxdIpDl7JnUl1Bdm/preview" allow="autoplay"></iframe>
            <div class="video-title">Video 14</div>
        </div>
        <div class="video-box" data-title="Ako-bluearchive-15">
            <iframe src="https://drive.google.com/file/d/1nBcmDAsPuyG51jdQhZaoyf9qs_ccg3Vj/preview" allow="autoplay"></iframe>
            <div class="video-title">Video 15</div>
        </div>
        <div class="video-box" data-title="Ako-bluearchive-16">
            <iframe src="https://drive.google.com/file/d/1tcNFY0H1LR7R-rJe8giBp_Gu5ymlzCTr/preview" allow="autoplay"></iframe>
            <div class="video-title">Video 16</div>
        </div>
        <div class="video-box" data-title="HonkaiImpact-17">
            <iframe src="https://drive.google.com/file/d/1zHMxni1xw4M3ba6b23BQ0LFiDStzFrzu/preview" allow="autoplay"></iframe>
            <div class="video-title">Video 17</div>
        </div>
        <div class="video-box" data-title="zzz-18">
            <iframe src="https://drive.google.com/file/d/1hb4aVfSIPCFGKyCrAwkHcVNB_nywrgNK/preview" allow="autoplay"></iframe>
            <div class="video-title">Video 18</div>
        </div>
        <div class="video-box" data-title="bronya-HonkaiImpact-19">
            <iframe src="https://drive.google.com/file/d/1GEFn7QOdNs-CMXdizLXL0BrkoIzmLshS/preview" allow="autoplay"></iframe>
            <div class="video-title">Video 19</div>
        </div>
        <div class="video-box" data-title="Rio-bluearchive-20">
            <iframe src="https://drive.google.com/file/d/1-yPonKgrsOkcouIhUZ4JYjESLn2wVSO9/preview" allow="autoplay"></iframe>
            <div class="video-title">Video 20</div>
        </div>
    </div>
    <div class="video-container" id="videoContainer1">
        <div class="video-box" data-title="zzz-burnice-caesar-21">
            <iframe src="https://drive.google.com/file/d/1qQ6oTviVxXnn9vTMyl0vQ41fEUCk95pl/preview" allow="autoplay"></iframe>
            <div class="video-title">Video 21</div>
        </div>
        <div class="video-box" data-title="wutheringwaves-camellya-22">
            <iframe src="https://drive.google.com/file/d/1Mdv24-cfquW8smdAR6TCcmXA7yNYUcXV/preview" allow="autoplay"></iframe>
            <div class="video-title">Video 22</div>
        </div>
        <div class="video-box" data-title="zzz-Miyabi-23">
            <iframe src="https://drive.google.com/file/d/10vZtMghpHgFbnG7_3aj2CJZ2rq-thfvM/preview" allow="autoplay"></iframe>
            <div class="video-title">Video 23</div>
        </div>
        <div class="video-box" data-title="Cat-24">
            <iframe src="https://drive.google.com/file/d/1NC-w-L4-hkZ-RzxKfn64onEquTagdKek/preview" allow="autoplay"></iframe>
            <div class="video-title">Video 24</div>
        </div>
        <div class="video-box" data-title="zzz-nicole-25">
            <iframe src="https://drive.google.com/file/d/1YUNQ56ILla7AL1WYJdSINtUWpeRXzqot/preview" allow="autoplay"></iframe>
            <div class="video-title">Video 25</div>
        </div>
        <div class="video-box" data-title="wutheringwaves-changli-26">
            <iframe src="https://drive.google.com/file/d/1aYQPDdGAXqFQNsWmRHunTG5GCpnWeTJR/preview" allow="autoplay"></iframe>
            <div class="video-title">Video 26</div>
        </div>
        <div class="video-box" data-title="HonkaiStaril-feixiao-27">
            <iframe src="https://drive.google.com/file/d/1r_cgoWPygzkDFaI4cSwFi7A7sYxWkvTV/preview" allow="autoplay"></iframe>
            <div class="video-title">Video 27</div>
        </div>
        <div class="video-box" data-title="fubuki-28">
            <iframe src="https://drive.google.com/file/d/1zc9-gOsnHb4zEndntBz5VpoiIw9QLrUR/preview" allow="autoplay"></iframe>
            <div class="video-title">Video 28</div>
        </div>
        <div class="video-box" data-title="HonkaiStaril-Tingyun-29">
            <iframe src="https://drive.google.com/file/d/1_xqOsDn_mmOQ4eo0Vymel5Jr8lnTolSc/preview" allow="autoplay"></iframe>
            <div class="video-title">Video 29</div>
        </div>
        <div class="video-box" data-title="Cat-30">
            <iframe src="https://drive.google.com/file/d/1T58M0-bt4I_hk6AyBcd5kQN66LV-A1nZ/preview" allow="autoplay"></iframe>
            <div class="video-title">Video 30</div>
        </div>

    <script>
        function filterVideos() {
            const searchInput = document.getElementById('searchInput').value.toLowerCase();
            const videoContainers = document.querySelectorAll('.video-container');

            videoContainers.forEach(container => {
                const videoBoxes = container.getElementsByClassName('video-box');
                for (let i = 0; i < videoBoxes.length; i++) {
                    const title = videoBoxes[i].getAttribute('data-title').toLowerCase();
                    if (title.includes(searchInput)) {
                        videoBoxes[i].style.display = 'block';
                    } else {
                        videoBoxes[i].style.display = 'none';
                    }
                }
            });
        }
    </script>

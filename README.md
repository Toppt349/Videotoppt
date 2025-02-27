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
        <div class="video-box" data-title="Machi">
            <iframe src="https://drive.google.com/file/d/1v_PcupEWHj-DZ1rC7CvMG0xh2Gge_TPU/preview" allow="autoplay"></iframe>
            <div class="video-title">Video 1</div>
        </div>

        <div class="video-box" data-title="HonkaiImpact">
            <iframe src="https://drive.google.com/file/d/1zpBDTn28jPtmZH59HgNXS-jToSoB2oOu/preview" allow="autoplay"></iframe>
            <div class="video-title">Video 2</div>
        </div>

        <div class="video-box" data-title="Mika-bluearchive">
            <iframe src="https://drive.google.com/file/d/1uBgqAHaDKggp6AyOXQ9oh0sZz6t18btH/preview" allow="autoplay"></iframe>
            <div class="video-title">Video 3</div>
        </div>

        <div class="video-box" data-title="Raiden-Genshin">
            <iframe src="https://drive.google.com/file/d/1AiLE5aP4VqSOMEUPcGYzrbbedEnnUxBa/preview" allow="autoplay"></iframe>
            <div class="video-title">Video 4</div>
        </div>
        
        <div class="video-box" data-title="Video 5">
            <iframe src="https://drive.google.com/file/d/1WuKp5qZcT_tnqD7gtVFiaXfavnnB1twf/preview" allow="autoplay"></iframe>
            <div class="video-title">Video 5</div>
        </div>

        <div class="video-box" data-title="Tosaka-Chicken">
            <iframe src="https://drive.google.com/file/d/10OUoaOaRNzervFJhp-rSroPuuW-Wh0pY/preview" allow="autoplay"></iframe>
            <div class="video-title">Video 6</div>
        </div>

        <div class="video-box" data-title="Tosaka-Chicken">
            <iframe src="https://drive.google.com/file/d/1lCb6oJbfDZZsfYFUkrq41b9Kp5609UO_/preview" allow="autoplay"></iframe>
            <div class="video-title">Video 7</div>
        </div>

        <div class="video-box" data-title="Vtuber">
            <iframe src="https://drive.google.com/file/d/1ZSPsXJd4mdecjMyhQHTNrZE8Q91BYJmd/preview" allow="autoplay"></iframe>
            <div class="video-title">Video 8</div>
        </div>

        <div class="video-box" data-title="Janedoe-zzz">
            <iframe src="https://drive.google.com/file/d/18ZDPA76vRGQecI_Xt_C6-2zh1OIhr3Pe/preview" allow="autoplay"></iframe>
            <div class="video-title">Video 9</div>
        </div>

        <div class="video-box" data-title="zzz">
            <iframe src="https://drive.google.com/file/d/1EK7C7XDORlEbTHPY_U1nBlhKmf-tGHo9/preview" allow="autoplay"></iframe>
            <div class="video-title">Video 10</div>
        </div>
    </div>

    <div class="video-container" id="videoContainer2">
        <div class="video-box" data-title="RaidenMei-Honkaistaril-Machi">
            <iframe src="https://drive.google.com/file/d/1e_9O1LALphMqZkdnYHLwfNoRhHeQ3JhE/preview" allow="autoplay"></iframe>
            <div class="video-title">Video 11</div>
        </div>
        <div class="video-box" data-title="Reelruru">
            <iframe src="https://drive.google.com/file/d/15V7eOeGesVKUPCFwpFuE_0O_LWCxhkNG/preview" allow="autoplay"></iframe>
            <div class="video-title">Video 12</div>
        </div>
        <div class="video-box" data-title="Ako-bluearchive">
            <iframe src="https://drive.google.com/file/d/1WPq7-dQW5XJTmBEznsTdJ76L4TLWhoQ0/preview" allow="autoplay"></iframe>
            <div class="video-title">Video 13</div>
        </div>
        <div class="video-box" data-title="Ako-bluearchive">
            <iframe src="https://drive.google.com/file/d/1AHE2gnyFb3Vk-tYjUxdIpDl7JnUl1Bdm/preview" allow="autoplay"></iframe>
            <div class="video-title">Video 14</div>
        </div>
        <div class="video-box" data-title="Ako-bluearchive">
            <iframe src="https://drive.google.com/file/d/1nBcmDAsPuyG51jdQhZaoyf9qs_ccg3Vj/preview" allow="autoplay"></iframe>
            <div class="video-title">Video 15</div>
        </div>
        <div class="video-box" data-title="Ako-bluearchive">
            <iframe src="https://drive.google.com/file/d/1tcNFY0H1LR7R-rJe8giBp_Gu5ymlzCTr/preview" allow="autoplay"></iframe>
            <div class="video-title">Video 16</div>
        </div>
        <div class="video-box" data-title="HonkaiImpact">
            <iframe src="https://drive.google.com/file/d/1zHMxni1xw4M3ba6b23BQ0LFiDStzFrzu/preview" allow="autoplay"></iframe>
            <div class="video-title">Video 17</div>
        </div>
        <div class="video-box" data-title="zzz">
            <iframe src="https://drive.google.com/file/d/1hb4aVfSIPCFGKyCrAwkHcVNB_nywrgNK/preview" allow="autoplay"></iframe>
            <div class="video-title">Video 18</div>
        </div>
        <div class="video-box" data-title="bronya-HonkaiImpact">
            <iframe src="https://drive.google.com/file/d/1GEFn7QOdNs-CMXdizLXL0BrkoIzmLshS/preview" allow="autoplay"></iframe>
            <div class="video-title">Video 19</div>
        </div>
        <div class="video-box" data-title="Rio-bluearchive">
            <iframe src="https://drive.google.com/file/d/1-yPonKgrsOkcouIhUZ4JYjESLn2wVSO9/preview" allow="autoplay"></iframe>
            <div class="video-title">Video 20</div>
        </div>
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

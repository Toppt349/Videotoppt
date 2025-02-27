
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

        .video-container {
            display: flex; /* ใช้ flexbox เพื่อให้วิดีโออยู่ในแถวเดียว */
            overflow-x: auto; /* ทำให้สามารถเลื่อนวิดีโอแนวนอนได้ */
            gap: 20px;
            padding-bottom: 20px; /* เพิ่มพื้นที่ด้านล่างเพื่อการเลื่อน */
        }

        .video-box {
            background: #202020;
            padding: 10px;
            border-radius: 10px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.3);
            transition: transform 0.3s ease;
            min-width: 320px; /* กำหนดความกว้างขั้นต่ำของแต่ละวิดีโอ */
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

        /* เพิ่ม Media Query สำหรับโทรศัพท์ */
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


    <h1>🎥 My Video Gallery</h1>

    <div class="video-container">
        <div class="video-box">
            <iframe src="https://drive.google.com/file/d/1v_PcupEWHj-DZ1rC7CvMG0xh2Gge_TPU/preview" allow="autoplay"></iframe>
            <div class="video-title">Video 1</div>
        </div>

        <div class="video-box">
            <iframe src="https://drive.google.com/file/d/1zpBDTn28jPtmZH59HgNXS-jToSoB2oOu/preview" allow="autoplay"></iframe>
            <div class="video-title">Video 2</div>
        </div>

        <div class="video-box">
            <iframe src="https://drive.google.com/file/d/1uBgqAHaDKggp6AyOXQ9oh0sZz6t18btH/preview" allow="autoplay"></iframe>
            <div class="video-title">Video 3</div>
        </div>

        <div class="video-box">
            <iframe src="https://drive.google.com/file/d/1AiLE5aP4VqSOMEUPcGYzrbbedEnnUxBa/preview" allow="autoplay"></iframe>
            <div class="video-title">Video 4</div>
        </div>
        
        <div class="video-box">
            <iframe src="https://drive.google.com/file/d/1WuKp5qZcT_tnqD7gtVFiaXfavnnB1twf/preview" allow="autoplay"></iframe>
            <div class="video-title">Video 5</div>
        </div>
    </div>
    <div class="video-container">
        <div class="video-box">
            <iframe src="https://drive.google.com/file/d/1v_PcupEWHj-DZ1rC7CvMG0xh2Gge_TPU/preview" allow="autoplay"></iframe>
            <div class="video-title">Video 1</div>
        </div>



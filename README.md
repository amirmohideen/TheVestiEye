# 👁️ The Vestibular Eye

**Using Snap Spectacles to make eye exercises fun, trackable, and effective.**

Built on Snap Spectacles, The Vestibular Eye transforms boring, unmonitored vestibular rehabilitation exercises into an engaging AR game where **your gaze is the controller**.

https://github.com/user-attachments/assets/082ebd1d-a57a-4ae3-9a92-beeb7d351651

## 💡 Inspiration

Vestibular Rehabilitation Therapy (VRT) is critical for recovery from balance and vestibular disorders — yet the exercises are notoriously repetitive, boring, and lonely. Doctors hand patients a sheet of paper and hope for the best. There is no feedback loop, no accountability, and no way to verify if a patient is performing the movements in the correct physiological range.

The Vestibular Eye changes that.

## 🚀 What It Does

- **Your Eye is the Cursor** - Spectacles' eye-tracking makes your gaze the controller.
- **The Gameplay Loop** - Guide a flying bird by keeping your gaze locked on it while moving your head through a specific path of targets.
- **Medical Verification** - To progress through levels, you must perform the movements correctly, ensuring patients hit the head-eye coordination benchmarks required for effective therapy.
- **Immediate Feedback** - Clear visual and audio cues give patients and doctors confidence that rehab is being done the right way.

## ⏩ What's Next

- **Doctor Dashboard** - Data logging so clinicians can remotely monitor patient accuracy and frequency.
- **Expanded Exercise Library** - New levels specifically designed for BPPV and other distinct vestibular conditions.
- **Enhanced "Juice"** - More immersive environments and particle effects to increase engagement and long-term compliance.

## 🛠️ Tech Stack

- **Platform:** <a href="https://developers.snap.com/lens-studio">Lens Studio</a> for Snap Spectacles
- **Language:** TypeScript
- **Eye Tracking:** Spectacles built-in eye-tracking API
- **Interaction:** <a href="https://developers.snap.com/spectacles/spectacles-frameworks/spectacles-interaction-kit/get-started">Spectacles Interaction Kit (SIK)</a>

## 📁 Architecture

| Script | Role |
| --- | --- |
| `RowController.ts` | Main game loop — manages target rows, progression logic, and level advancement |
| `PinchStartButton.ts` | Handles the pinch gesture to start or restart the experience |
| `CollisionHider.ts` | Hides objects on collision events (e.g., when a target is successfully hit) |
| `DistanceHider.ts` | Shows/hides objects based on gaze distance thresholds |

## 🔧 Setup

### Prerequisites

- <a href="https://developers.snap.com/lens-studio">Lens Studio 5.4+</a>
- Snap Spectacles (or the Lens Studio preview for testing)

### Clone the Repository

```bash
git clone https://github.com/amirmohideen/TheVestiEye.git
cd TheVestiEye
```

### Open in Lens Studio

1. Launch **Lens Studio**.
2. Select **File → Open Project**.
3. Navigate to the cloned folder and open **`TheVestiEye.esproj`**.
4. Lens Studio will load the scene and all assets automatically.

### Build & Run

- **On Spectacles:** Connect your Spectacles, then click **Push to Device** in Lens Studio.
- **In Preview:** Use Lens Studio's built-in preview mode to test gaze and interaction logic without a physical device.

## 🤝 Contributing

Contributions are welcome! Whether you want to add new exercise levels, improve the feedback system, or build out the doctor dashboard - open an issue or pull request.

1. Fork the repo
2. Create a feature branch: `git checkout -b feature/your-feature`
3. Commit your changes: `git commit -m "Add your feature"`
4. Push and open a Pull Request

## 📄 License

MIT


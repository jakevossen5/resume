all : resume.pdf jake-vossen-resume.pdf jake-vossen-cv.pdf

jake-vossen-cv.pdf : fonts/FontAwesome.ttf fonts/Roboto-Bold.ttf fonts/Roboto-BoldItalic.ttf fonts/Roboto-Italic.ttf fonts/Roboto-Light.ttf fonts/Roboto-LightItalic.ttf fonts/Roboto-Medium.ttf fonts/Roboto-MediumItalic.ttf fonts/Roboto-Regular.ttf fonts/Roboto-Thin.ttf fonts/Roboto-ThinItalic.ttf awesome-cv.cls fontawesome.sty cv/education.tex cv/experience.tex cv/skills.tex cv.tex cv/honors.tex cv/extracurricular.tex base.tex

	xelatex cv.tex
	mv cv.pdf jake-vossen-cv.pdf

jake-vossen-resume.pdf : resume.pdf
	cp resume.pdf jake-vossen-resume.pdf

resume.pdf : fonts/FontAwesome.ttf fonts/Roboto-Bold.ttf fonts/Roboto-BoldItalic.ttf fonts/Roboto-Italic.ttf fonts/Roboto-Light.ttf fonts/Roboto-LightItalic.ttf fonts/Roboto-Medium.ttf fonts/Roboto-MediumItalic.ttf fonts/Roboto-Regular.ttf fonts/Roboto-Thin.ttf fonts/Roboto-ThinItalic.ttf awesome-cv.cls fontawesome.sty cv/education.tex cv/experience.tex cv/skills.tex cv.tex cv/honors.tex cv/extracurricular.tex base.tex
	xelatex resume.tex


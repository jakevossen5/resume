all : jake-vossen-resume.pdf resume.pdf cv.org

jake-vossen-resume.pdf : resume.pdf
	cp resume.pdf jake-vossen-resume.pdf

resume.pdf : fonts/FontAwesome.ttf fonts/Roboto-Bold.ttf fonts/Roboto-BoldItalic.ttf fonts/Roboto-Italic.ttf fonts/Roboto-Light.ttf fonts/Roboto-LightItalic.ttf fonts/Roboto-Medium.ttf fonts/Roboto-MediumItalic.ttf fonts/Roboto-Regular.ttf fonts/Roboto-Thin.ttf fonts/Roboto-ThinItalic.ttf awesome-cv.cls fontawesome.sty resume/education.tex resume/experience.tex resume/skills.tex resume.tex resume/honors.tex resume/extracurricular.tex
	xelatex resume.tex


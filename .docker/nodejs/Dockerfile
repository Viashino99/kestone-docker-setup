FROM node:20.11.0-alpine

RUN apk add --no-cache \
	bash \
	busybox-extras \
	htop \
	libc6-compat \
	fzf \
	git \
	ncdu 

RUN corepack enable && corepack prepare pnpm@8.14.0 --activate

WORKDIR /var/app

ENV PORT 3000

USER node

CMD ["sh", "run-dev.sh"]

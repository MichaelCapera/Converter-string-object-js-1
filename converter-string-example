/**
 * Starts the resolver execution
 * @param {import('@aws-appsync/utils').Context} ctx the context
 * @returns {*} the return value sent to the first AppSync function
 */
export function request(ctx) {
console.log('ObjectString', ctx.arguments.stringObject);
const str = ctx.arguments.stringObject;
console.log('String ==>', str);
const convertedStr = str.split("'").join('\\\"');
console.log('Converted string ==>', convertedStr);
const strOne = `${convertedStr}`;
console.log('StrOne ==>', strOne);
console.log('CTX ==>', ctx);
  return {};

}

/**
 * Returns the resolver result
 * @param {import('@aws-appsync/utils').Context} ctx the context
 * @returns {*} the return value of the last AppSync function response handler
 */
export function response(ctx) {
  return {itemData:'Ok'};
}